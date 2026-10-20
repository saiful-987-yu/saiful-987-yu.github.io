<div align="center">

# 🏘️ আমাদের এলাকা · Amader Elaka

**ড্রাইভার, ডাক্তার, দোকান, মসজিদ ও জরুরি সেবা — আপনার এলাকার সব ফোন নম্বর এক জায়গায়।**
*Drivers, doctors, shops, mosques and emergency services — your area's contacts in one place.*

[🌐 ওয়েবসাইট খুলুন · Open the site](https://saiful-987-yu.github.io/amader-elaka/)

</div>

---

## 📌 এই রিপোজিটরি কী? · What is this repository?

এটি `saiful-987-yu.github.io` ডোমেইনের **রুট (root) রিপোজিটরি**। এখানে কোনো ওয়েবসাইটের কোড নেই। এর একমাত্র কাজ হলো **আমাদের এলাকা** অ্যান্ড্রয়েড অ্যাপকে এই ডোমেইনের সাথে যাচাই (verify) করা, যাতে অ্যাপ খুললে ব্রাউজারের অ্যাড্রেস বার ছাড়া ফুল-স্ক্রিন অ্যাপের মতো চলে।

This is the **root repository** of the `saiful-987-yu.github.io` domain. It holds no website code. Its only job is to verify the **Amader Elaka** Android app against this domain (Digital Asset Links), so the app opens full-screen without a browser address bar.

> মূল ওয়েবসাইট ও সব সোর্স কোড আছে আলাদা রিপোজিটরিতে: **`amader-elaka`**
> The actual website and its source code live in the separate **`amader-elaka`** repository.

---

## 🗂️ ফাইল ও ফোল্ডার · Files

| পথ · Path | কাজ · Purpose |
|---|---|
| `.well-known/assetlinks.json` | অ্যাপ ও ডোমেইনের মধ্যে যাচাইয়ের ফাইল · App ↔ domain verification file |
| `.nojekyll` | GitHub Pages-কে `.well-known` ফোল্ডার প্রকাশ করতে দেয় · Lets GitHub Pages publish the `.well-known` folder |
| `README.md` | এই ডকুমেন্ট · This document |

⚠️ **`.well-known` ফোল্ডার ও `.nojekyll` ফাইল কখনো মুছবেন না।** মুছলে অ্যাপে আবার অ্যাড্রেস বার দেখা যাবে।
**Never delete `.well-known` or `.nojekyll`.** Without them the app will show the browser address bar again.

---

## 📱 অ্যান্ড্রয়েড অ্যাপের তথ্য · Android app details

| বিষয় · Item | মান · Value |
|---|---|
| অ্যাপের নাম · App name | Amader Elaka |
| Package ID | `io.github.saiful987yu.amaderelaka` |
| ধরন · Type | Trusted Web Activity (TWA), [PWABuilder](https://www.pwabuilder.com) দিয়ে তৈরি · built with PWABuilder |
| লোড হয় · Loads | `https://saiful-987-yu.github.io/amader-elaka/` |
| Signing certificate SHA-256 | `38:2F:15:11:C7:50:95:CF:29:8E:FB:B0:08:84:4D:7F:5E:36:6E:C1:E1:5E:3D:44:62:0C:6A:18:39:2F:99:B6` |

এই fingerprint গোপন তথ্য নয়, এটি `assetlinks.json`-এ প্রকাশ্যে থাকাই নিয়ম।
This fingerprint is not a secret; it is meant to be public inside `assetlinks.json`.

---

## 🔄 আপডেট কীভাবে কাজ করে · How updates work

অ্যাপটি তৈরি করা হয়েছে লাইভ ওয়েবসাইটের উপর, তাই:

- ✅ `amader-elaka` রিপোজিটরিতে সাইট আপডেট করলেই সবার অ্যাপে নতুন সংস্করণ চলে আসে। নতুন APK বানানো বা বিলি করার দরকার নেই।
- ✅ নতুন কোড বা ডিজাইন ইনস্টল করা অ্যাপে নিজে থেকেই দেখা যায়।
- 🔁 নতুন APK লাগে কেবল অ্যাপের নাম, আইকন, package বা signing key বদলালে।

The app wraps the live website, so:

- ✅ Updating the site in the `amader-elaka` repository updates every installed app. No new APK is needed.
- 🔁 A new APK is only needed if the app name, icon, package ID or signing key changes.

---

## 🔐 নিরাপত্তা নির্দেশনা · Security notes

| ✅ করুন · Do | ❌ করবেন না · Don't |
|---|---|
| `signing.keystore` ও `signing-key-info.txt` নিজের কাছে নিরাপদে ব্যাকআপ রাখুন | এই দুই ফাইল GitHub বা অন্য কোথাও আপলোড/শেয়ার করবেন না |
| `assetlinks.json`-এর package ও fingerprint ঠিক রাখুন | অ্যাপ ও key না বদলে এই ফাইল এডিট করবেন না |
| APK শুধু নির্ভরযোগ্য লিংক থেকে শেয়ার করুন | কীস্টোর পাসওয়ার্ড কাউকে দেবেন না |

Keep the keystore backed up privately. If it is lost, future updates of the same app can no longer be signed.

---

## 🧪 যাচাই করুন · Verify the setup

নিচের লিংকটি ব্রাউজারে খুললে `assetlinks.json`-এর লেখা দেখা যাবে:

```
https://saiful-987-yu.github.io/.well-known/assetlinks.json
```

ফাইলটি খোলা না গেলে দেখুন: রিপোজিটরি **Public** আছে কি না, **Settings → Pages**-এ `main` ব্রাঞ্চ চালু আছে কি না, এবং `.nojekyll` ফাইলটি আছে কি না।

---

## 🛠️ সমস্যা ও সমাধান · Troubleshooting

| সমস্যা · Problem | সমাধান · Fix |
|---|---|
| অ্যাপে উপরে অ্যাড্রেস বার দেখা যাচ্ছে | উপরের লিংকে `assetlinks.json` খোলে কি না দেখুন। খুললে ফোনের Settings → Apps → Amader Elaka থেকে ডেটা ক্লিয়ার করে অ্যাপ আবার খুলুন |
| `assetlinks.json` খুলছে না (404) | `.nojekyll` আছে কি না এবং Pages চালু আছে কি না দেখুন; আপলোডের পর এক-দুই মিনিট অপেক্ষা করুন |
| package বা fingerprint মিলছে না | `assetlinks.json`-এর মান ও APK-এর package/key একই কি না মিলিয়ে নিন |
| পুরোনো APK ইনস্টল হচ্ছে না | আগের ইনস্টল করা অ্যাপ মুছে নতুন APK ইনস্টল করুন (key আলাদা হলে এমন হয়) |

---

<div align="center">

**আমাদের এলাকা** — স্থানীয় মানুষের জন্য, স্থানীয় তথ্য।
🌐 [saiful-987-yu.github.io/amader-elaka](https://saiful-987-yu.github.io/amader-elaka/)

</div>
