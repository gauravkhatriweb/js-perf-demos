
# ⚡ 7-Line Speed-Run: Cut 2.1 s TTI Without Rewrites

> Your app feels sluggish because these 7 lines are silently killing it.  
> I shaved 2.1 s off **Time-to-Interactive** in production with the same checklist—**no rewrites, just micro-optimisations**.

---

## 📋 The 7-Step Checklist I Keep Pinned in VS Code

| # | Micro-Optimisation | Impact |
|---|--------------------|--------|
| **1** | **Loop swap** → `for` beats `forEach` by ~30 % in Node | Faster hot paths |
| **2** | **Debounce scroll** → 16 ms instead of 250 ms wasted reflows | Smoother UX |
| **3** | **Tree-shake** → `import { debounce } from 'lodash-es'` cut **124 KB** | Smaller bundle |
| **4** | **Lazy load routes** → `React.lazy(() => import('./Admin'))` dropped initial JS by **38 %** | Faster FCP |
| **5** | **Time with precision** → `performance.now()` pinpointed a **22 ms leak** in a closure | Accurate profiling |
| **6** | **Batch DOM edits** → `requestAnimationFrame` + `DocumentFragment` = zero layout thrash | Reflow-free renders |
| **7** | **Cleanup listeners** → Removing resize listeners in `useEffect` cleanup saved **12 MB RAM** after 50 route changes | Memory-safe SPA |

---


## 🔗 Quick Links

- **Benchmark Repo** → [github.com/gauravkhatriweb/js-perf-demos](https://github.com/gauravkhatriweb/js-perf-demos)  
- **My GitHub** → [github.com/gauravkhatriweb](https://github.com/gauravkhatriweb)  
- **My LinkedIn** → [linkedin.com/in/gauravkhatriweb](https://linkedin.com/in/gauravkhatriweb)

---

## 🤝 Contribute

Got a faster tweak or new benchmark?  
Open an issue or PR—tag `@gauravkhatriweb`.

---

## 🪪 License

MIT © [Gaurav Khatri](https://github.com/gauravkhatriweb)
