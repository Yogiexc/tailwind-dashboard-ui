# ⚡ Tailwind CSS Quick Reference

> Cheatsheet untuk utility classes yang sering digunakan

## 🎨 Layout

### Display
```html
<div class="block">           <!-- display: block -->
<div class="inline-block">    <!-- display: inline-block -->
<div class="flex">            <!-- display: flex -->
<div class="inline-flex">     <!-- display: inline-flex -->
<div class="grid">            <!-- display: grid -->
<div class="hidden">          <!-- display: none -->
```

### Flexbox
```html
<!-- Direction -->
<div class="flex-row">        <!-- flex-direction: row -->
<div class="flex-col">        <!-- flex-direction: column -->

<!-- Justify Content -->
<div class="justify-start">   <!-- justify-content: flex-start -->
<div class="justify-center">  <!-- justify-content: center -->
<div class="justify-between"> <!-- justify-content: space-between -->
<div class="justify-around">  <!-- justify-content: space-around -->

<!-- Align Items -->
<div class="items-start">     <!-- align-items: flex-start -->
<div class="items-center">    <!-- align-items: center -->
<div class="items-end">       <!-- align-items: flex-end -->
<div class="items-stretch">   <!-- align-items: stretch -->
```

### Grid
```html
<div class="grid grid-cols-1">    <!-- 1 column -->
<div class="grid grid-cols-2">    <!-- 2 columns -->
<div class="grid grid-cols-3">    <!-- 3 columns -->
<div class="grid grid-cols-4">    <!-- 4 columns -->

<div class="gap-4">               <!-- gap: 1rem -->
<div class="gap-6">               <!-- gap: 1.5rem -->
```

---

## 📏 Spacing

### Padding
```html
<div class="p-0">    <!-- padding: 0 -->
<div class="p-1">    <!-- padding: 0.25rem (4px) -->
<div class="p-2">    <!-- padding: 0.5rem (8px) -->
<div class="p-4">    <!-- padding: 1rem (16px) -->
<div class="p-6">    <!-- padding: 1.5rem (24px) -->
<div class="p-8">    <!-- padding: 2rem (32px) -->

<!-- Directional -->
<div class="px-4">   <!-- padding-left, padding-right -->
<div class="py-2">   <!-- padding-top, padding-bottom -->
<div class="pt-4">   <!-- padding-top -->
<div class="pr-4">   <!-- padding-right -->
<div class="pb-4">   <!-- padding-bottom -->
<div class="pl-4">   <!-- padding-left -->
```

### Margin
```html
<div class="m-0">    <!-- margin: 0 -->
<div class="m-4">    <!-- margin: 1rem -->
<div class="m-auto"> <!-- margin: auto -->

<!-- Directional -->
<div class="mx-auto"> <!-- margin-left: auto, margin-right: auto -->
<div class="my-4">    <!-- margin-top, margin-bottom -->
<div class="mt-4">    <!-- margin-top -->
<div class="mr-4">    <!-- margin-right -->
<div class="mb-4">    <!-- margin-bottom -->
<div class="ml-4">    <!-- margin-left -->

<!-- Negative margins -->
<div class="-mt-4">   <!-- margin-top: -1rem -->
```

---

## 📐 Sizing

### Width
```html
<div class="w-0">       <!-- width: 0 -->
<div class="w-px">      <!-- width: 1px -->
<div class="w-1">       <!-- width: 0.25rem -->
<div class="w-full">    <!-- width: 100% -->
<div class="w-screen">  <!-- width: 100vw -->
<div class="w-1/2">     <!-- width: 50% -->
<div class="w-1/3">     <!-- width: 33.333% -->
<div class="w-1/4">     <!-- width: 25% -->

<!-- Max/Min Width -->
<div class="max-w-xs">  <!-- max-width: 20rem -->
<div class="max-w-sm">  <!-- max-width: 24rem -->
<div class="max-w-md">  <!-- max-width: 28rem -->
<div class="max-w-lg">  <!-- max-width: 32rem -->
<div class="max-w-xl">  <!-- max-width: 36rem -->
```

### Height
```html
<div class="h-full">    <!-- height: 100% -->
<div class="h-screen">  <!-- height: 100vh -->
<div class="h-12">      <!-- height: 3rem (48px) -->
<div class="h-16">      <!-- height: 4rem (64px) -->

<!-- Min Height -->
<div class="min-h-screen"> <!-- min-height: 100vh -->
```

---

## 🎨 Colors

### Background
```html
<div class="bg-white">      <!-- Pure white -->
<div class="bg-black">      <!-- Pure black -->
<div class="bg-gray-50">    <!-- Lightest gray -->
<div class="bg-gray-500">   <!-- Mid gray -->
<div class="bg-gray-900">   <!-- Darkest gray -->

<div class="bg-blue-500">   <!-- Blue -->
<div class="bg-red-500">    <!-- Red -->
<div class="bg-green-500">  <!-- Green -->
<div class="bg-yellow-500"> <!-- Yellow -->
<div class="bg-purple-500"> <!-- Purple -->

<!-- Transparency -->
<div class="bg-blue-500/50">  <!-- 50% opacity -->
<div class="bg-blue-500/75">  <!-- 75% opacity -->
```

### Text Color
```html
<div class="text-gray-900">   <!-- Dark text -->
<div class="text-gray-600">   <!-- Medium text -->
<div class="text-gray-400">   <!-- Light text -->
<div class="text-blue-600">   <!-- Blue text -->
```

### Border Color
```html
<div class="border-gray-200">
<div class="border-blue-500">
```

---

## 🔤 Typography

### Font Size
```html
<div class="text-xs">     <!-- 0.75rem (12px) -->
<div class="text-sm">     <!-- 0.875rem (14px) -->
<div class="text-base">   <!-- 1rem (16px) -->
<div class="text-lg">     <!-- 1.125rem (18px) -->
<div class="text-xl">     <!-- 1.25rem (20px) -->
<div class="text-2xl">    <!-- 1.5rem (24px) -->
<div class="text-3xl">    <!-- 1.875rem (30px) -->
<div class="text-4xl">    <!-- 2.25rem (36px) -->
```

### Font Weight
```html
<div class="font-thin">       <!-- 100 -->
<div class="font-light">      <!-- 300 -->
<div class="font-normal">     <!-- 400 -->
<div class="font-medium">     <!-- 500 -->
<div class="font-semibold">   <!-- 600 -->
<div class="font-bold">       <!-- 700 -->
<div class="font-extrabold">  <!-- 800 -->
```

### Text Align
```html
<div class="text-left">
<div class="text-center">
<div class="text-right">
<div class="text-justify">
```

### Line Height
```html
<div class="leading-none">    <!-- 1 -->
<div class="leading-tight">   <!-- 1.25 -->
<div class="leading-normal">  <!-- 1.5 -->
<div class="leading-relaxed"> <!-- 1.625 -->
<div class="leading-loose">   <!-- 2 -->
```

---

## 🎯 Borders

### Border Width
```html
<div class="border">      <!-- 1px all sides -->
<div class="border-0">    <!-- No border -->
<div class="border-2">    <!-- 2px all sides -->
<div class="border-4">    <!-- 4px all sides -->

<!-- Directional -->
<div class="border-t">    <!-- top -->
<div class="border-r">    <!-- right -->
<div class="border-b">    <!-- bottom -->
<div class="border-l">    <!-- left -->
```

### Border Radius
```html
<div class="rounded-none">    <!-- 0 -->
<div class="rounded-sm">      <!-- 0.125rem (2px) -->
<div class="rounded">         <!-- 0.25rem (4px) -->
<div class="rounded-md">      <!-- 0.375rem (6px) -->
<div class="rounded-lg">      <!-- 0.5rem (8px) -->
<div class="rounded-xl">      <!-- 0.75rem (12px) -->
<div class="rounded-2xl">     <!-- 1rem (16px) -->
<div class="rounded-full">    <!-- 9999px -->

<!-- Directional -->
<div class="rounded-t-lg">    <!-- top -->
<div class="rounded-r-lg">    <!-- right -->
<div class="rounded-b-lg">    <!-- bottom -->
<div class="rounded-l-lg">    <!-- left -->
```

---

## ✨ Effects

### Box Shadow
```html
<div class="shadow-sm">   <!-- Subtle shadow -->
<div class="shadow">      <!-- Default shadow -->
<div class="shadow-md">   <!-- Medium shadow -->
<div class="shadow-lg">   <!-- Large shadow -->
<div class="shadow-xl">   <!-- Extra large shadow -->
<div class="shadow-none"> <!-- No shadow -->
```

### Opacity
```html
<div class="opacity-0">     <!-- Invisible -->
<div class="opacity-25">    <!-- 25% visible -->
<div class="opacity-50">    <!-- 50% visible -->
<div class="opacity-75">    <!-- 75% visible -->
<div class="opacity-100">   <!-- Fully visible -->
```

---

## 🎬 Transitions

### Transition Property
```html
<div class="transition">          <!-- All properties -->
<div class="transition-colors">   <!-- Color properties -->
<div class="transition-opacity">  <!-- Opacity -->
<div class="transition-shadow">   <!-- Shadow -->
<div class="transition-transform"><!-- Transform -->
```

### Duration
```html
<div class="duration-75">    <!-- 75ms -->
<div class="duration-100">   <!-- 100ms -->
<div class="duration-150">   <!-- 150ms -->
<div class="duration-200">   <!-- 200ms -->
<div class="duration-300">   <!-- 300ms -->
<div class="duration-500">   <!-- 500ms -->
```

### Timing Function
```html
<div class="ease-linear">
<div class="ease-in">
<div class="ease-out">
<div class="ease-in-out">
```

---

## 🎭 Pseudo-Classes

### Hover
```html
<button class="bg-blue-500 hover:bg-blue-700">
  Hover me
</button>
```

### Focus
```html
<input class="border focus:border-blue-500 focus:ring-2">
```

### Active
```html
<button class="active:bg-blue-800">
  Click me
</button>
```

### Disabled
```html
<button class="disabled:opacity-50 disabled:cursor-not-allowed" disabled>
  Disabled
</button>
```

---

## 📱 Responsive Design

### Breakpoints
```html
<!-- Mobile first -->
<div class="w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/6">

<!-- Breakpoint reference:
  sm: 640px
  md: 768px
  lg: 1024px
  xl: 1280px
  2xl: 1536px
-->
```

### Example Patterns
```html
<!-- Stack on mobile, side-by-side on desktop -->
<div class="flex flex-col md:flex-row">

<!-- Hide on mobile, show on desktop -->
<div class="hidden md:block">

<!-- Show on mobile, hide on desktop -->
<div class="block md:hidden">

<!-- Different padding per breakpoint -->
<div class="p-4 md:p-6 lg:p-8">
```

---

## 🌙 Dark Mode

```html
<!-- Setup in config -->
<!-- darkMode: 'class' in tailwind.config.js -->

<!-- Usage -->
<div class="bg-white dark:bg-gray-800 
            text-gray-900 dark:text-white">
  Content adapts to theme
</div>

<button class="text-gray-600 dark:text-gray-300 
               hover:text-gray-900 dark:hover:text-white">
  Button
</button>
```

---

## 🎯 Common Patterns

### Centered Content
```html
<div class="flex items-center justify-center min-h-screen">
  Vertically & horizontally centered
</div>
```

### Card
```html
<div class="bg-white rounded-lg shadow-md p-6 
            hover:shadow-lg transition-shadow">
  Card content
</div>
```

### Button
```html
<button class="px-4 py-2 bg-blue-600 text-white rounded-lg 
               hover:bg-blue-700 transition-colors">
  Click me
</button>
```

### Badge
```html
<span class="px-3 py-1 text-xs font-medium bg-green-100 
             text-green-700 rounded-full">
  Active
</span>
```

### Avatar
```html
<div class="w-10 h-10 rounded-full bg-blue-500 
            flex items-center justify-center 
            text-white font-semibold text-sm">
  JD
</div>
```

---

## 🔧 Custom Values

### Arbitrary Values
```html
<!-- Use when design tokens don't fit -->
<div class="w-[347px]">        <!-- Custom width -->
<div class="top-[117px]">      <!-- Custom position -->
<div class="bg-[#bada55]">     <!-- Custom color -->
<div class="text-[17px]">      <!-- Custom size -->

<!-- ⚠️ Use sparingly! Prefer design tokens -->
```

---

## 💡 Pro Tips

### 1. Group Related Classes
```html
<!-- ✅ Good: Grouped by concern -->
<div class="
  flex items-center
  w-full h-12
  px-4 py-2
  bg-white
  rounded-lg
  shadow-md
">
```

### 2. Mobile-First
```html
<!-- ✅ Start with mobile, add desktop -->
<div class="w-full md:w-1/2 lg:w-1/3">

<!-- ❌ Don't start with desktop -->
<div class="lg:w-1/3 md:w-1/2 w-full">
```

### 3. Use @apply Sparingly
```css
/* Only for repeated patterns */
@layer components {
  .btn {
    @apply px-4 py-2 rounded-lg font-medium;
  }
}
```

### 4. Consistent Spacing
```html
<!-- ✅ Use scale: 0, 1, 2, 4, 6, 8, 12, 16 -->
<div class="p-4 mb-6 mt-8">

<!-- ❌ Don't use arbitrary -->
<div class="p-[17px] mb-[23px]">
```

---

## 📚 Resources

- [Official Docs](https://tailwindcss.com/docs)
- [Tailwind Play](https://play.tailwindcss.com/) - Online playground
- [Tailwind UI](https://tailwindui.com/) - Component library
- [Heroicons](https://heroicons.com/) - Icon library

---

**Keep this handy while coding! 🚀**