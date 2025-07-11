# VS Code Custom Snippet for Auto-Named React TypeScript Component

## 🚀 Overview

এই Snippet দিয়ে আপনি সহজেই VS Code এ React TypeScript functional component অটো জেনারেট করতে পারবেন, যেখানে component এর নাম হবে ফাইলের নাম অনুযায়ী। 

---

## 🛠️ Setup Instructions

### Step 1: Open Snippet File

VS Code এ নিচের কাজ করুন:

- `Ctrl + Shift + P` প্রেস করুন
- সার্চ বক্সে লিখুন `Snippets: Configure User Snippets`
- সিলেক্ট করুন `typescriptreact.json` (React TS ফাইলের জন্য)

---

### Step 2: Snippet কোড পেস্ট করুন

`typescriptreact.json` ফাইলে নিচের কোড পেস্ট করুন:

```json
{
  "Custom Functional Component (cc)": {
    "prefix": "cc",
    "body": [
      "const $TM_FILENAME_BASE = () => {",
      "  return (",
      "    <div>",
      "      <h1>This is $TM_FILENAME_BASE component</h1>$0",
      "    </div>",
      "  );",
      "};",
      "",
      "export default $TM_FILENAME_BASE;"
    ],
    "description": "TypeScript Functional Component with cc"
  }
}
```