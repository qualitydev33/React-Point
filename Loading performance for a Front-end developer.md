# Loading performance for a Front-end developer

For Web developers, performance isn’t optional now. Performance plays a major role in the success of any online venture. DoubleClick by Google found 53% of mobile site visits were abandoned if a page took longer than 3 seconds to load.

## Improving performance
In this post, I am jotting down some loading performance techniques helpful for Web developers to consider while building websites/web apps.

## Setting up Performance Budget
A performance budget is a limit for pages which the team is not allowed to exceed. It could be a max JavaScript bundle size, total image weight, a specific load time (e.g Time-to-Interactive in under 5s on 3G/4G) or threshold on any number of other metrics.

## 1. JavaScript

*   Consider implementing [code-splitting](https://webpack.js.org/guides/code-splitting/)
*   [Trim your JavaScript bundles](https://nolanlawson.com/2018/03/20/smaller-lodash-bundles-with-webpack-and-babel/)
*   [Prioritize resources with Preload](https://developers.google.com/web/fundamentals/performance/resource-prioritization), [Preconnect](https://developers.google.com/web/fundamentals/performance/resource-prioritization), [Prefetch](https://developers.google.com/web/fundamentals/performance/resource-prioritization)
*   [Reduce JavaScript Payloads with Tree Shaking](https://developers.google.com/web/fundamentals/performance/optimizing-javascript/tree-shaking/)
*   [Embrace performance budgets](https://infrequently.org/2017/10/can-you-afford-it-real-world-web-performance-budgets/)

## 2. Images
*   Appropriate image format
*   Appropriate compression method
*   Appropriate for display size and density according to viewport/device
*   Load only necessary — lazy loaded

### Techniques/guides
*   [images.guide](https://images.guide/)
*   [Image Optimization](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization)
*   [SVG Will Save Us](https://svgontheweb.com/)
*   [Lazy loading](https://developers.google.com/web/fundamentals/performance/lazy-loading-guidance/images-and-video/) — [Native image](https://addyosmani.com/blog/lazy-loading/) lazy-loading is coming for the web.

## 3. Fonts
*   [Controlling Font Performance with font-display](https://developers.google.com/web/updates/2016/02/font-display)
*   font-display [for the Masses](https://css-tricks.com/font-display-masses/)

## 4. Converting website/app to PWAs
Progressive Web Apps are experiences that combine the best of the web and the best of apps. — Google Web

Using these experiences we can build reliable, fast and engaging websites/web apps. [Service workers](https://developers.google.com/web/fundamentals/primers/service-workers/) enable a Progressive Web App to load instantly, regardless of the network state. The service worker is like a client-side proxy, allows to control the cache and how to respond to resource requests.

See [Top 5 Service Worker Essentials](https://www.youtube.com/watch?v=IBpQlNeq5-o&index=3&list=PLNYkxOF6rcIDjlCx1PcphPpmf43aKOAdF&t=0s) for Web Developers Youtube video from Chrome Dev Summit 2018.

## 5. Choose suitable rendering techniques, pattern
*   [Rendering on the Web](https://developers.google.com/web/updates/2019/02/rendering-on-the-web)
*   [The PRPL Pattern](https://developers.google.com/web/fundamentals/performance/prpl-pattern/)
*   [Architect your App Shell](https://codelabs.developers.google.com/codelabs/your-first-pwapp/#2)

## 6. Some other techniques
*   [HTTP Caching](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching)
*   [Optimizing Encoding](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer)

## 7. Tooling
*   [Chrome dev tool](https://developers.google.com/web/tools/chrome-devtools/) — Audit, Performance, Memory, JavaScript profiler, Coverage, Performance monitor, Network
*   [Lighthouse](https://developers.google.com/web/tools/lighthouse/)
*   [Webpagetest](https://www.webpagetest.org/)
*   [Pagespeed](https://developers.google.com/speed/pagespeed/module/)