---
theme: apple-basic
layout: intro
transition: slide-left
---

# Vite

<h2>下一代的前端工具链</h2>

<div class="image-box"></div>
<img  src="https://cn.vitejs.dev/logo-with-shadow.png" />

<div @click="$slidev.nav.next" class="button px-2 py-1 rounded cursor-pointer" hover="bg-opacity-10">
  开始
</div>

<style>
.button {
  width: 100px;
  height: 30px;
  line-height: 23px;
  text-align: center;
  margin-top: 30px;
  color: #fff;
  background-color: #646cff;
}

h1, h2 {
  background: -webkit-linear-gradient( 120deg, #bd34fe 30%, #41d1ff );
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
  font-weight: 700;
  white-space: pre-wrap;
}

h2 {
  margin-top: 30px;
}

.image-box {
  position: absolute;
  top: 50%;
  left: 70%;
  border-radius: 50%;
  width: 320px;
  height: 320px;
  background-image: linear-gradient( -45deg, #bd34fe 50%, #47caff 50% );
  filter: blur(40px);
  transform: translate(-50%,-50%);
}

img {
  position: absolute;
  top: 50%;
  left: 70%;
  transform: translate(-50%,-50%);
  width: 200px;
  height: 200px;
}

</style>

---
highlighter: shiki
transition: slide-up
---

## 为什么选择 Vite

<li v-click class="text-xl p-2 slidev-vclick-target"> 无论项目大小有多大，启动应用都只需更少的时间； </li>
<li v-click class="text-xl p-2 slidev-vclick-target"> 按需编译； </li>
<li v-click class="text-xl p-2 slidev-vclick-target"> 零配置，开箱即用； </li>
<li v-click class="text-xl p-2 slidev-vclick-target"> Esbuild 能力带来的 Typescript/jsx 的原生支持 </li>

<li v-click class="text-xl p-2 slidev-vclick-target svg">
<svg viewBox="0 0 1896 1071" fill="none" xmlns="http://www.w3.org/2000/svg">
<text fill="#FFAA3E" xml:space="preserve" style="white-space: pre" font-size="80" letter-spacing="0em"><tspan x="45" y="129.344">Native ESM based dev server</tspan></text>
<rect x="632" y="526" width="273" height="106" rx="10" fill="#C3E88C"></rect>
<text fill="#15505C" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="724.5" y="591.988">entry</tspan></text>
<rect x="1106" y="699" width="274" height="114" rx="10" fill="#666665"></rect>
<g filter="url(#filter0_d_5_61)">
<text fill="#CCCCCB" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0.33em"><tspan x="1213.5" y="768.988">···</tspan></text>
</g>
<rect x="1106" y="346" width="274" height="113" rx="10" fill="#4FC08D"></rect>
<text fill="#15505C" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="1198" y="415.488">route</tspan></text>
<rect x="1102" y="524" width="273" height="114" rx="10" fill="#666665"></rect>
<text fill="#CCCCCB" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="1193.5" y="593.988">route</tspan></text>
<path d="M1101.79 402.463L1067.99 410.054L1091.46 435.529L1101.79 402.463ZM910.168 583.106L1083.96 422.965L1079.9 418.553L906.102 578.693L910.168 583.106Z" fill="#C892E9"></path>
<path d="M1097 581L1067 563.679V598.321L1097 581ZM908 584H1070V578H908V584Z" fill="#999899"></path>
<path d="M1101.79 756.57L1091.2 723.584L1067.93 749.242L1101.79 756.57ZM906.119 583.121L1079.77 740.651L1083.8 736.207L910.151 578.677L906.119 583.121Z" fill="#999899"></path>
<path d="M1552.72 948.839L1545.7 914.916L1519.83 937.953L1552.72 948.839ZM1381.73 761.331L1532.52 930.67L1537 926.68L1386.21 757.341L1381.73 761.331Z" fill="#999899"></path>
<path d="M1549.95 756.569L1541.94 722.868L1516.76 746.659L1549.95 756.569ZM1381.79 582.96L1529.23 739.005L1533.59 734.884L1386.15 578.839L1381.79 582.96Z" fill="#999899"></path>
<path d="M1547.19 585.049L1517.64 566.972L1516.76 601.602L1547.19 585.049ZM1383.89 583.898L1520.12 587.362L1520.27 581.364L1384.04 577.9L1383.89 583.898Z" fill="#999899"></path>
<path d="M1548.57 402.463L1519.02 384.386L1518.14 419.015L1548.57 402.463ZM1385.27 401.312L1521.5 404.776L1521.66 398.778L1385.43 395.314L1385.27 401.312Z" fill="#C892E9"></path>
<path d="M631.489 585.049L601.583 567.567L601.396 602.207L631.489 585.049ZM375.576 586.666L604.473 587.903L604.506 581.903L375.608 580.666L375.576 586.666Z" fill="#C892E9"></path>
<path d="M1549.95 219.877L1516.97 230.462L1542.63 253.735L1549.95 219.877ZM1390.34 400.329L1534.04 241.892L1529.59 237.861L1385.89 396.298L1390.34 400.329Z" fill="#C892E9"></path>
<path d="M1547.19 573.983L1539.89 540.12L1514.21 563.372L1547.19 573.983ZM1385.89 400.327L1526.84 555.983L1531.29 551.956L1390.34 396.3L1385.89 400.327Z" fill="#C892E9"></path>
<rect x="1553" y="152" width="274" height="113" rx="10" fill="#4FC08D"></rect>
<text fill="#15505C" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="1626" y="221.488">module</tspan></text>
<rect x="1553" y="341" width="274" height="114" rx="10" fill="#4FC08D"></rect>
<text fill="#15505C" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="1621.5" y="411.818">module</tspan></text>
<rect x="1550" y="517" width="274" height="114" rx="10" fill="#666665"></rect>
<text fill="#CCCCCB" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="1623" y="586.988">module</tspan></text>
<rect x="1553" y="707" width="274" height="113" rx="10" fill="#666665"></rect>
<text fill="#CCCCCB" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="1626" y="776.488">module</tspan></text>
<rect x="1553" y="896" width="274" height="113" rx="10" fill="#666665"></rect>
<text fill="#CCCCCB" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0.33em"><tspan x="1660.5" y="965.488">···</tspan></text>
<rect x="45" y="491" width="330" height="179" rx="10" fill="#029788"></rect>
<text fill="white" xml:space="preserve" style="white-space: pre" font-size="38" font-weight="600" letter-spacing="0em"><tspan x="154.707" y="570.988">Server
</tspan><tspan x="162.76" y="615.988">ready</tspan></text>
<line x1="507.615" y1="459.201" x2="506.232" y2="569.859" stroke="#C892E9" stroke-width="4" stroke-dasharray="8 8"></line>
<line x1="1038.78" y1="733.073" x2="1037.37" y2="883.845" stroke="#E06666" stroke-width="4" stroke-dasharray="8 8"></line>
<text fill="#E06666" xml:space="preserve" style="white-space: pre" font-size="38" letter-spacing="0em"><tspan x="918" y="938.988">Dynamic import
</tspan><tspan x="918" y="983.988">(code split point)</tspan></text>
<text fill="#C892E9" xml:space="preserve" style="white-space: pre" font-size="38" letter-spacing="0em"><tspan x="399" y="431.488">HTTP request</tspan></text>
<defs>
<filter id="filter0_d_5_61" x="1212.15" y="752.766" width="60.9863" height="13.2324" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
<feFlood flood-opacity="0" result="BackgroundImageFix"></feFlood>
<feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"></feColorMatrix>
<feOffset dy="4"></feOffset>
<feGaussianBlur stdDeviation="2"></feGaussianBlur>
<feComposite in2="hardAlpha" operator="out"></feComposite>
<feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"></feColorMatrix>
<feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_5_61"></feBlend>
<feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_5_61" result="shape"></feBlend>
</filter>
</defs>
</svg>
</li>

<style>
.svg {
    width: 400px;
    height: 300px;
}

</style>

---
transition: slide-up
---

## 创建第一个 Vite 项目

使用 NPM:

```ts
$ npm create vite@latest
```

使用 Yarn:

```ts
$ yarn create vite
```

使用 Yarn:·

```ts
$ yarn create vite

$ yarn create v1.22.10
$ [1/4] 🔍  Resolving packages...
$ [2/4] 🚚  Fetching packages...
$ [3/4] 🔗  Linking dependencies...
$ [4/4] 🔨  Building fresh packages..
```

```ts {monaco}
? Project name: › vite-project
```

---
transition: slide-out
---

## 选择模板

```ts 
? Select a framework: › - Use arrow-keys. Return to submit.
    Vanilla
❯   Vue
    React
    Preact
    Lit
    Svelte
    Others
```
选择语言

```ts
? Select a variant: › - Use arrow-keys. Return to submit.
❯   JavaScript
    TypeScript
    Customize with create-vue ↗
    Nuxt ↗

```
运行

```ts
Done. Now run:
  cd my-porject
  yarn
  yarn dev
```  
---
transition: slide-up
---

## 进入项目

```json
{
  "name": "my-porject",
  "private": true,
  "version": "0.0.0",
  "type": "module",
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  },
  "dependencies": {
    "vue": "^3.2.45"
  },
  "devDependencies": {
    "@vitejs/plugin-vue": "^4.0.0",
    "vite": "^4.1.0"
  }
}
```
<img
  v-click
  class="absolute arrow w-80 opacity-50"
  src="https://sli.dev/assets/arrow-bottom-left.svg"
/>


<style>
.arrow {
  left: 3.75rem;
  right: 18.5rem;;
}

</style>