`aspect` is a replacement for the `bazel` CLI that comes with Bazel.
It provides a simpler, more intutive experience for developers new to Bazel,
while also adding the power tools that make advanced users more productive.

## Interactive

When running in an interactive terminal, `aspect` helps you out.

<script id="asciicast-eL4HL3BZhobRD8U4UIRKzyb8R" src="https://asciinema.org/a/eL4HL3BZhobRD8U4UIRKzyb8R.js" async></script>

It can
- offer to fix problems that block your developers
- suggest better ways to use the tool

## Customize for your organization with plugins

Every organization has a different engineering culture and developer stack.

![People working together on software](/people.png)

Bazel was designed for Google's workflows, not yours.

A plugin allows you to fit `aspect` into your teams development process. For example, you can:
- stamp out new Bazel projects following your local conventions
- point error messages to your internal documentation
- add commands for deploying, linting, rebasing, or other common developer workflows
- understand where your developers get stuck and provide help

A vibrant ecosystem of plugins accelerates your Bazel migration.
For example, Aspect has written a plugin to augment error messages:

<script id="asciicast-57gaElVKNlb0d8pyZ7JGBDZhL" src="https://asciinema.org/a/57gaElVKNlb0d8pyZ7JGBDZhL.js" async></script>

Plugins are any program, written in any language, that runs a gRPC server speaking our protocol. We use the [plugin system from HashiCorp](https://github.com/hashicorp/go-plugin).

Read more: [Plugins documentation](/help/topics/plugins)

## Open source and no lock-in

You can rely on aspect-cli to power your developer experience workflows.

It is free and open-source. It is a superset of what Bazel provides,
so you can always go back to running `bazel` commands.

## Expert help is a click away

aspect-cli is sponsored by Aspect Development, a Bazel consulting company.
If your organization needs more help to make your Bazel migration a success,
come find us at [aspect.dev](https://aspect.dev)

# Installation:

## Using a package manager

Coming soon

## Manual installation

Download a binary from our [GitHub Releases] page and put it in your PATH.

On MacOS you can bypass the "Unknown Developer" dialog by running
`xattr -c $(which aspect)` before launching aspect.

# User Manuals

The commands are documented under [aspect](/aspect).

[Bazel]: http://bazel.build
[GitHub Releases]: https://github.com/aspect-dev/aspect-cli/releases
