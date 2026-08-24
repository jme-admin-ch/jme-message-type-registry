# JME Message Type Registry

See [Message Type Registry](https://jeap-admin-ch.github.io/docs/building-blocks/libraries/jeap-messaging/message-type-registry)
for details on the message type registry format and tooling.

This message type registry contains the message types produced or consumed by the JME example services: commands
under `descriptor/jme/command/` (e.g. `jmecreatedeclarationcommand`) and events under `descriptor/jme/event/`
(e.g. `jmeordercreatedevent`, `jmeracestartedevent`). Each message type is a folder with one `.avdl` file per
published version; `descriptor/jme/_common/` holds Avro definitions shared across multiple message types (e.g.
`DocumentReference`, `OrderReference`). `jme-message-contract-service` and the various example services in this
GitHub organization resolve their message schemas from this registry.

## Note

This repository is part of the open source distribution of jEAP. See [github.com/jeap-admin-ch/jeap](https://github.com/jeap-admin-ch/jeap)
for more information.

## License

This repository is Open Source Software licensed under the [Apache License 2.0](./LICENSE).
