<div align="center">

Hi 👋 I'm **Yuki Yamazaki**(a.k.a. kamiazya).

🔗

[![Zenn](https://img.shields.io/badge/zenn-kamiazya?style=flat&logo=zenn&logoColor=fff&labelColor=3EA8FF&color=3EA8FF)](https://zenn.dev/kamiazya)
[![Speaker Deck](https://img.shields.io/badge/Speaker_Deck-kamiazya?style=flat&logo=speakerdeck&logoColor=fff&labelColor=009287&color=009287)](https://speakerdeck.com/kamiazya/)
[![X](https://img.shields.io/badge/X-kamiazya?style=flat&logo=x&logoColor=fff&labelColor=000&color=000)](https://x.com/kamiazya)
[![npm](https://img.shields.io/badge/npm-kamiazya?style=flat&logo=npm&logoColor=fff&labelColor=CB3837&color=CB3837)](https://www.npmjs.com/~kamiazya)
[![Keybase](https://img.shields.io/badge/keybase-kamiazya?style=flat&logo=keybase&logoColor=fff&labelColor=33A0FF&color=33A0FF)
](https://keybase.io/kamiazya)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-kamiazya?style=flat&logo=linkedin&logoColor=fff&labelColor=0A66C2&color=0A66C2)](https://www.linkedin.com/in/kamiazya/)

<details>
<summary>As is... 🔍</summary>

##### Professional Role 💼
I currently work as a data engineer and front-end engineer at [iRidge, Inc.](https://iridge.jp/), where I specialize in developing and maintaining mobile application support kits.

##### Open Source Contributions 🌐
In my free time, I passionately contribute to open-source software projects. One of my notable projects is the [ts-graphviz](https://github.com/ts-graphviz) library, which receives around 2 million downloads monthly.

![NPM Downloads](https://img.shields.io/npm/dm/ts-graphviz)  

</details>

<details>
<summary>To be... 🎯</summary>

##### Future Goals 🚀

My aspiration is to transition into a full-time role dedicated to contributing to my favorite open-source projects. 

I aim to leverage my skills and experience to make a significant impact in the open-source community.

##### Sponsorship 🤝

Your support as a sponsor would be greatly appreciated and would enable me to continue enhancing the quality and security of open-source software.

[![GitHub Sponsor](https://img.shields.io/badge/-GitHub%20Sponsor-fff?logo=GitHub%20Sponsors&style=flat)](https://github.com/sponsors/kamiazya)
[![OpenCollective](https://img.shields.io/badge/-OpenCollective-7FADF2?logoColor=fff&logo=opencollective&style=flat)](https://opencollective.com/kamiazya)

</details>

</div>

---

## Projects 🚀

### Featured Projects 🌟

#### [rediagram](https://github.com/kamiazya/rediagram)

A tool for creating **architecture diagrams using [React](https://react.dev/)**, providing an easy and efficient way to visualize your system architecture.

<details>
<summary>Open 📖</summary>

Code your system architecture in the style of React, JSX/TSX.

[MyInfra.rediagram.tsx](https://github.com/kamiazya/rediagram/examples/gallery/src/MyInfra.rediagram.tsx)

```tsx
import React from 'react';
import { PNG, Diagram, GeneralIcon } from 'rediagram';
import { AWS, InvizAWS, EC2, Lambda, Region, SecurityGroup, AutoScalingGroup } from '@rediagram/aws';

PNG(
  <Diagram title="My Infra">
    <InvizAWS>
      <AWS>
        <Region name="Asia Pacific (Tokyo)">
          <AutoScalingGroup>
            <EC2 name="REST API" type="Instance" upstream={['worker4']} />
          </AutoScalingGroup>
          <SecurityGroup>
            <Lambda name="worker4" type="Lambda Function" upstream={['worker5', 'worker6']} />
            <Lambda name="worker5" type="Lambda Function" />
            <Lambda name="worker6" type="Lambda Function" />
          </SecurityGroup>
        </Region>
      </AWS>
      <GeneralIcon name="Browser" type="Client" upstream={['REST API']} />
    </InvizAWS>
  </Diagram>,
);
```

Running this file will generate a diagram of `MyInfra.rediagram.png`.

```bash
$ ts-node MyInfra.rediagram.tsx
```

</details>

![Image](https://raw.githubusercontent.com/kamiazya/rediagram/master/examples/gallery/img/MyInfra.rediagram.png)


<div align="center">

![GitHub Repo stars](https://img.shields.io/github/stars/kamiazya/rediagram?style=flat)

</div>

#### [web-csv-toolbox](https://github.com/kamiazya/web-csv-toolbox)

A set of tools for managing and manipulating CSV files on the web. It relies solely on Web standard APIs and experimentally supports WebAssembly (WASM) for enhanced performance.

<div align="center">

![GitHub Repo stars](https://img.shields.io/github/stars/kamiazya/web-csv-toolbox?style=flat)
[![NPM Version](https://img.shields.io/npm/v/web-csv-toolbox)](https://www.npmjs.com/package/web-csv-toolbox)
[![NPM Downloads](https://img.shields.io/npm/dm/web-csv-toolbox)](https://www.npmjs.com/package/web-csv-toolbox)

</div>

### [ts-graphviz](https://github.com/ts-graphviz) Organization 📊

<div align="center">

![](https://avatars.githubusercontent.com/u/63964583?s=100)

[![GitHub Sponsor](https://img.shields.io/badge/-GitHub%20Sponsor-fff?logo=GitHub%20Sponsors&style=flat)](https://github.com/sponsors/ts-graphviz)
[![OpenCollective](https://img.shields.io/badge/-OpenCollective-7FADF2?logoColor=fff&logo=opencollective&style=flat)](https://opencollective.com/ts-graphviz)
![GitHub Org's stars](https://img.shields.io/github/stars/ts-graphviz)

</div>

The `ts-graphviz` organization is dedicated to developing tools and libraries that enhance the use of [Graphviz](https://graphviz.gitlab.io/) with [TypeScript](https://www.typescriptlang.org/).
Our projects aim to simplify and streamline the creation, visualization, and management of graph structures, making it easier for developers to integrate powerful graph visualization capabilities into their applications.

| Repository | Description | Badges |
| --- | --- | --- |
| [ts-graphviz](https://github.com/ts-graphviz/ts-graphviz) | Simple Graphviz library for TypeScript. | [![NPM Version](https://img.shields.io/npm/v/ts-graphviz)](https://www.npmjs.com/package/ts-graphviz) [![NPM Downloads](https://img.shields.io/npm/dm/ts-graphviz)](https://www.npmjs.com/package/ts-graphviz) ![GitHub Repo stars](https://img.shields.io/github/stars/ts-graphviz/ts-graphviz?style=flat) |
| [setup-graphviz](https://github.com/ts-graphviz/setup-graphviz) | A GitHub Action to easily set up Graphviz in your CI environment. It simplifies the installation process and helps maintain consistency across different development setups. | ![GitHub Repo stars](https://img.shields.io/github/stars/ts-graphviz/setup-graphviz?style=flat) |
| [prettier-plugin-dot](https://github.com/ts-graphviz/prettier-plugin-dot) | A Prettier plugin for the DOT language used by Graphviz, enabling automatic code formatting for DOT files. | [![NPM Version](https://img.shields.io/npm/v/prettier-plugin-dot)](https://www.npmjs.com/package/prettier-plugin-dot) [![NPM Downloads](https://img.shields.io/npm/dm/prettier-plugin-dot)](https://www.npmjs.com/package/prettier-plugin-dot) ![GitHub Repo stars](https://img.shields.io/github/stars/ts-graphviz/prettier-plugin-dot?style=flat) |

### Other Projects 💻

> These projects enhance development workflows and documentation processes, addressing various needs within the developer community.

#### [typedoc-plugin-mermaid](https://github.com/kamiazya/typedoc-plugin-mermaid)

A plugin for [TypeDoc](https://typedoc.org/) that integrates [Mermaid](https://mermaid.js.org/) diagrams. It enhances documentation by allowing the inclusion of flowcharts, sequence diagrams, and more, directly within TypeDoc-generated documentation.

<div align="center">

[![NPM Version](https://img.shields.io/npm/v/typedoc-plugin-mermaid)](https://www.npmjs.com/package/typedoc-plugin-mermaid)
[![NPM Downloads](https://img.shields.io/npm/dm/typedoc-plugin-mermaid)](https://www.npmjs.com/package/typedoc-plugin-mermaid)
![GitHub Repo stars](https://img.shields.io/github/stars/kamiazya/typedoc-plugin-mermaid?style=flat)

</div>

#### [ulauncher-vivaldi-profiles](https://github.com/kamiazya/ulauncher-vivaldi-profiles)

A [Ulauncher](https://ulauncher.io/) extension that allows you to switch between different [Vivaldi](https://vivaldi.com/) browser profiles easily.

![](https://raw.githubusercontent.com/kamiazya/ulauncher-vivaldi-profiles/main/screenshot.png)

<div align="center">

![GitHub Repo stars](https://img.shields.io/github/stars/kamiazya/ulauncher-vivaldi-profiles?style=flat)

</div>

### Work In Progress 🛠️

> These ongoing projects aim to simplify complex tasks and integrate advanced features. Stay tuned for updates as they evolve.

| Repository | Description |
| --- | --- |
| [connectable-io](https://github.com/kamiazya/connectable-io) | Connectable IO offers unified interfaces for various resources, including storage, logging, queues, and more. By abstracting these resources, it enables seamless interactions across different solutions and protocols, simplifying integration and usage. |
| [vue-highlight](https://github.com/kamiazya/vue-highlight) | Vue 3+ directive for highlighting keywords in text. This directive allows you to highlight matching keywords within a given element using your own CSS. It leverages the [Custom Highlighting API](https://developer.mozilla.org/en-US/docs/Web/API/CSS_Custom_Highlight_API) to avoid corrupting the DOM, though this API is not supported by all browsers​. |
