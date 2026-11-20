# Awesome Viva

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of applications, tools and resources for [Viva](https://github.com/vivaui/viva), a Go-first, GPU-native desktop framework.

Viva draws native windows and GPU surfaces on macOS, Windows and Linux with no
WebView, no browser engine and no bundled runtime. Applications are written in
Go, components are source-distributed, and a release binary carries only the
code it uses.

English | [简体中文](README.zh-CN.md)

## Contents

- [Applications](#applications)
- [Official resources](#official-resources)
- [Framework packages](#framework-packages)
- [Tooling](#tooling)
- [Learning](#learning)
- [Community](#community)
- [Contributing](#contributing)
- [Licence](#licence)

## Applications

Applications built with Viva whose source is public.

- [Motty](https://github.com/t8y2/motty) - An SSH workspace with a terminal, SFTP, port forwarding, remote desktops and an AI assistant in one native window. `macOS` `Windows` `Linux` · Apache-2.0
- [Peck](https://github.com/eryajf/Peck) - A macOS menu bar assistant that inspects quarantine and code-signing state, then opens a blocked app after you confirm. `macOS` · Apache-2.0
- [Tinglan](https://github.com/talongao/tinglan) - An unofficial, experimental Huawei Music client with a native library, lyrics, twelve themes and a dockable player. `macOS` · AGPL-3.0
- [Viff](https://github.com/1lck/viff) - A lightweight native Git client with line staging, side-by-side diffs and paginated history. `macOS` `Windows` · MIT
- [GoIM](https://github.com/Ezreal-byte/GoIM) - A desktop messenger with automatic device discovery, direct and group chat, and file sharing over a local network. `macOS` `Windows` `Linux` · MIT

## Official resources

- [Viva](https://github.com/vivaui/viva) - The framework and runtime: a Go module for macOS, Windows and Linux.
- [Website](https://vivaui.dev/en/) - Guides, the API reference and the component catalog, with live previews. Also [in Chinese](https://vivaui.dev/zh/).
- [Documentation](https://vivaui.dev/en/docs/) - Every guide, from the first window to packaging.
- [API reference](https://vivaui.dev/en/api/) - The public Go API, package by package.
- [Component catalog](https://vivaui.dev/en/components/) - The source-distributed recipes rendered with live previews.
- [Showcase](https://vivaui.dev/en/showcase/) - Applications built with Viva, with screenshots and links.
- [Releases](https://github.com/vivaui/viva/releases) - Release notes, source tags and prebuilt `viva` command archives.

## Framework packages

- [app](https://pkg.go.dev/github.com/vivaui/viva/app) - Window lifecycle, status items, secrets, drag and drop, and platform services.
- [ui](https://pkg.go.dev/github.com/vivaui/viva/ui) - Retained scene, paint primitives, input, focus and accessibility.
- [flex](https://pkg.go.dev/github.com/vivaui/viva/flex) - CSS-flexbox-style layout declared in Go.
- [components](https://pkg.go.dev/github.com/vivaui/viva/components) - shadcn-inspired recipes; one plain Go file per component.
- [text](https://pkg.go.dev/github.com/vivaui/viva/text) - Text shaping and editing contracts.
- [markdown](https://pkg.go.dev/github.com/vivaui/viva/markdown) - Native rendering for the Markdown that assistants and release notes use.
- [headless](https://pkg.go.dev/github.com/vivaui/viva/headless) - Runs an application's real paint, input and focus paths without a window.

## Tooling

- [viva command](https://github.com/vivaui/viva/tree/main/cmd/viva) - Builds, packages, initializes and live-reloads applications; none of it is linked into a release binary.
- [Homebrew tap](https://github.com/vivaui/homebrew-tap) - `brew install vivaui/tap/viva` on macOS and Linux.
- [Scoop manifests](https://github.com/vivaui/homebrew-tap) - The same repository holds the Windows manifests: `scoop bucket add vivaui ...`.
- [Headless testing](https://vivaui.dev/en/docs/testing/) - The `vivahead` build tag and the harness that never opens a window.
- [Coding-agent skill](https://github.com/vivaui/viva/tree/main/docs/skills/building-with-viva) - A skill file that teaches an agent the programming model and the headless workflow.

## Learning

- [Getting started](https://vivaui.dev/en/docs/getting-started/) - Install the command, initialize a project, open a window.
- [Programming model](https://vivaui.dev/en/docs/programming-model/) - State, invalidation and repaint.
- [Declarative layout](https://vivaui.dev/en/docs/declarative-layout/) - Build a page from values instead of coordinates.
- [Drawing and layout](https://vivaui.dev/en/docs/drawing-and-layout/) - The paint path and how layout fits in it.
- [Handling input](https://vivaui.dev/en/docs/handling-input/) - Pointer, keyboard and focus.
- [Text input](https://vivaui.dev/en/docs/text-input/) - Native editing, selection and input methods.
- [Theming](https://vivaui.dev/en/docs/theming/) - Colors, type and density.
- [Build and package](https://vivaui.dev/en/docs/build-and-package/) - From `viva build` to a signed bundle.
- [Testing](https://vivaui.dev/en/docs/testing/) - Drive the UI headlessly in `go test`.
- [Performance](https://vivaui.dev/en/docs/performance/) - The budgets and how they are measured.
- [Platforms](https://vivaui.dev/en/docs/platforms/) - What each backend supports today.
- [System integration](https://vivaui.dev/en/docs/system-integration/) - Status items, secrets, file drops and the file manager.

## Community

- [Discussions](https://github.com/vivaui/viva/discussions) - Questions, ideas and show-and-tell.
- [Issues](https://github.com/vivaui/viva/issues) - Bug reports and feature requests.
- [Contributing](https://github.com/vivaui/viva/blob/main/CONTRIBUTING.md) - How changes to the framework are reviewed.
- [Code of conduct](https://github.com/vivaui/viva/blob/main/CODE_OF_CONDUCT.md)

## Contributing

Missing something? Add it.

This list follows the [Awesome](https://awesome.re) conventions. To add an
application, edit both `README.md` and `README.zh-CN.md` in one pull request and:

- link an application that uses Viva for its own UI, not as a wrapper around a web page;
- keep one entry per project, in the existing order;
- provide a public source repository with build or install instructions, an explicit licence and signs of maintenance;
- write one sentence about what the application does and who it is for.

The full checklist is in [CONTRIBUTING.md](CONTRIBUTING.md).

## Licence

[![CC0](https://licensebuttons.net/p/zero/1.0/80x15.png)](https://creativecommons.org/publicdomain/zero/1.0/)

The list itself is released under CC0 1.0. Names, code and artwork belong to
their respective projects.
