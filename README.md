name: Template
description: Plugin Description
version: 1.0
main: me.eduard.template.Main
authors: [Eduard]
commands:
  comando:
    aliases: [aliases,as]
    permission: perm.use
    permission-message: No Permission
    usage: /<command>
    description: Comando Description
  pluginperm.*:
    default: op
    description: Permission OP
    children:
      pluginperm.plugintp: true
      pluginperm.plugingo: true
  pluginperm.plugintp:
    default: op
    description: Permission TP
  pluginperm.plugingo:
    default: op
    description: Permission Go
