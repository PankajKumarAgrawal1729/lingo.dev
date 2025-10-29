<p align="center">
  <a href="https://lingo.dev">
    <img
      src="https://raw.githubusercontent.com/lingodotdev/lingo.dev/main/content/banner.compiler.png"
      width="100%"
      alt="Lingo.dev"
    />
  </a>
</p>

<p align="center">
  <strong>
    ⚡ Lingo.dev - মুক্ত উৎস, AI-চালিত i18n টুলকিট LLM ৰ সৈতে তৎক্ষণাৎ 
    স্থানীয়কৰণৰ বাবে।
  </strong>
</p>

<br />

<p align="center">
  <a href="https://lingo.dev/compiler">Lingo.dev কম্পাইলাৰ</a> •
  <a href="https://lingo.dev/cli">Lingo.dev CLI</a> •
  <a href="https://lingo.dev/ci">Lingo.dev CI/CD</a> •
  <a href="https://lingo.dev/sdk">Lingo.dev SDK</a>
</p>

<p align="center">
  <a href="https://github.com/lingodotdev/lingo.dev/actions/workflows/release.yml">
    <img
      src="https://github.com/lingodotdev/lingo.dev/actions/workflows/release.yml/badge.svg"
      alt="মুক্তি"
    />
  </a>
  <a href="https://github.com/lingodotdev/lingo.dev/blob/main/LICENSE.md">
    <img
      src="https://img.shields.io/github/license/lingodotdev/lingo.dev"
      alt="অনুমতিপত্ৰ"
    />
  </a>
  <a href="https://github.com/lingodotdev/lingo.dev/commits/main">
    <img
      src="https://img.shields.io/github/last-commit/lingodotdev/lingo.dev"
      alt="শেষ কমিট"
    />
  </a>
  <a href="https://lingo.dev/en">
    <img src="https://img.shields.io/badge/Product%20Hunt-%231%20DevTool%20of%20the%20Month-orange?logo=producthunt&style=flat-square" alt="Product Hunt #1 DevTool of the Month" />
  </a>
  <a href="https://lingo.dev/en">
    <img src="https://img.shields.io/badge/Product%20Hunt-%231%20Product%20of%20the%20Week-orange?logo=producthunt&style=flat-square" alt="Product Hunt #1 DevTool of the Week" />
  </a>
  <a href="https://lingo.dev/en">
    <img src="https://img.shields.io/badge/Product%20Hunt-%232%20Product%20of%20the%20Day-orange?logo=producthunt&style=flat-square" alt="Product Hunt #2 Product of the Day" />
  </a>
  <a href="https://lingo.dev/en">
    <img src="https://img.shields.io/badge/GitHub-Trending-blue?logo=github&style=flat-square" alt="Github trending" />
  </a>
</p>

---

## কম্পাইলাৰৰ সৈতে পৰিচয় 🆕

**Lingo.dev কম্পাইলাৰ** এটা বিনামূলীয়া, মুক্ত উৎসৰ কম্পাইলাৰ মিডলৱেৰ, যি বৰ্তমানৰ React উপাদানসমূহত কোনো পৰিৱৰ্তন নকৰাকৈ নিৰ্মাণ সময়ত যিকোনো React এপ্পক বহুভাষিক কৰিবলৈ ডিজাইন কৰা হৈছে।

এবাৰ ইনষ্টল কৰক:

```bash
npm install lingo.dev
```

আপোনাৰ নিৰ্মাণ কনফিগত সক্ষম কৰক:

```js
import lingoCompiler from "lingo.dev/compiler";

const existingNextConfig = {};

export default lingoCompiler.next({
  sourceLocale: "en",
  targetLocales: ["es", "fr"],
})(existingNextConfig);
```

`next build` চলাওক আৰু স্পেনিছ আৰু ফৰাচী বাণ্ডল ওলাই অহা চাওক ✨

[ডকুমেণ্টেচন পঢ়ক →](https://lingo.dev/compiler) সম্পূৰ্ণ গাইডৰ বাবে, আৰু [আমাৰ Discord ত যোগদান কৰক](https://lingo.dev/go/discord) আপোনাৰ চেটআপত সহায় পাবলৈ।

---

### এই ৰেপোত কি আছে?

| টুল          | চমু বিৱৰণ                                                                     | ডকুমেণ্টেচন                           |
| ------------ | ------------------------------------------------------------------------------ | --------------------------------------- |
| **কম্পাইলাৰ** | নিৰ্মাণ-সময়ৰ React স্থানীয়কৰণ                                               | [/compiler](https://lingo.dev/compiler) |
| **CLI**      | ৱেব আৰু মোবাইল এপ্প, JSON, YAML, মাৰ্কডাউনৰ বাবে এক-আদেশৰ স্থানীয়কৰণ     | [/cli](https://lingo.dev/cli)           |
| **CI/CD**    | প্ৰতিটো পুছত স্বয়ংক্ৰিয় অনুবাদ কমিট + প্ৰয়োজন অনুসৰি পুল অনুৰোধ সৃষ্টি      | [/ci](https://lingo.dev/ci)             |
| **SDK**      | ব্যৱহাৰকাৰী-সৃষ্ট বিষয়বস্তুৰ বাবে প্ৰকৃত সময়ৰ অনুবাদ                       | [/sdk](https://lingo.dev/sdk)           |

তলত প্ৰতিটোৰ বাবে দ্ৰুত তথ্য দিয়া হৈছে 👇

---

### ⚡️ Lingo.dev CLI

আপোনাৰ টাৰ্মিনেলৰ পৰা পোনপটীয়াকৈ কোড আৰু বিষয়বস্তু অনুবাদ কৰক।

```bash
npx lingo.dev@latest run
```

ই প্ৰতিটো ষ্ট্ৰিং ফিংগাৰপ্ৰিণ্ট কৰে, ফলাফল কেশ কৰে, আৰু কেৱল সলনি হোৱা কথাবোৰহে পুনৰ অনুবাদ কৰে।

[ডকুমেণ্ট অনুসৰণ কৰক →](https://lingo.dev/cli) ইয়াক কেনেকৈ চেটআপ কৰিব লাগে জানিবলৈ।

---

### 🔄 Lingo.dev CI/CD

স্বয়ংক্ৰিয়ভাৱে নিখুঁত অনুবাদ শিপ কৰক।

```yaml
# .github/workflows/i18n.yml
name: Lingo.dev i18n
on: [push]

jobs:
  i18n:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: lingodotdev/lingo.dev@main
        with:
          api-key: ${{ secrets.LINGODOTDEV_API_KEY }}
```

আপোনাৰ ৰেপো সেউজীয়া আৰু আপোনাৰ উৎপাদন হস্তচালিত পদক্ষেপ অবিহনে বহুভাষিক ৰাখে।

[ডকুমেণ্টেচন পঢ়ক →](https://lingo.dev/ci)

---

### 🧩 Lingo.dev SDK

গতিশীল বিষয়বস্তুৰ বাবে তৎক্ষণাৎ প্ৰতি-অনুৰোধ অনুবাদ।

```ts
import { LingoDotDevEngine } from "lingo.dev/sdk";

const lingoDotDev = new LingoDotDevEngine({
  apiKey: "your-api-key-here",
});

const content = {
  greeting: "Hello",
  farewell: "Goodbye",
  message: "Welcome to our platform",
};

const translated = await lingoDotDev.localizeObject(content, {
  sourceLocale: "en",
  targetLocale: "es",
});
// Returns: { greeting: "Hola", farewell: "Adiós", message: "Bienvenido a nuestra plataforma" }
```

চেট, ব্যৱহাৰকাৰীৰ মন্তব্য, আৰু অন্যান্য প্ৰকৃত-সময়ৰ প্ৰবাহৰ বাবে নিখুঁত।

[ডকুমেণ্টেচন পঢ়ক →](https://lingo.dev/sdk)

---

## 🤝 সম্প্ৰদায়

আমি সম্প্ৰদায়-চালিত আৰু অৱদান ভাল পাওঁ!

- কোনো ধাৰণা আছে? [এটা ইছু খোলক](https://github.com/lingodotdev/lingo.dev/issues)
- কিবা ঠিক কৰিব বিচাৰে? [এটা PR পঠিয়াওক](https://github.com/lingodotdev/lingo.dev/pulls)
- সহায় লাগে? [আমাৰ Discord ত যোগদান কৰক](https://lingo.dev/go/discord)

## ⭐ তৰকা ইতিহাস

যদি আমাৰ কাম আপোনাৰ ভাল লাগে, আমাক এটা ⭐ দিয়ক আৰু 4,000 তৰকা পোৱাত সহায় কৰক! 🌟

[![তৰকা ইতিহাস চাৰ্ট](https://api.star-history.com/svg?repos=lingodotdev/lingo.dev&type=Date)](https://www.star-history.com/#lingodotdev/lingo.dev&Date)

## 🌐 অন্যান্য ভাষাত Readme

[English](https://github.com/lingodotdev/lingo.dev) • [中文](/readme/zh-Hans.md) • [日本語](/readme/ja.md) • [한국어](/readme/ko.md) • [Español](/readme/es.md) • [Français](/readme/fr.md) • [Русский](/readme/ru.md) • [Українська](/readme/uk-UA.md) • [Deutsch](/readme/de.md) • [Italiano](/readme/it.md) • [العربية](/readme/ar.md) • [עברית](/readme/he.md) • [हिन्दी](/readme/hi.md) • [বাংলা](/readme/bn.md) • [فارسی](/readme/fa.md) • [অসমীয়া](/readme/as.md)

আপোনাৰ ভাষা দেখা নাই? [`i18n.json`](./i18n.json) ত যোগ দিয়ক আৰু এটা PR খোলক!