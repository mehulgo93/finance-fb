<!-- This project uses route groups in Next Js.
Most of the code is written in the app folder and if you make a new folder and use page.tsx you need to do export default instead of export const
route group means you can use parenthesis inside a folder in order to not use the name of the folder in the link.
Authentication is written using the square brackets, this gives you access to all routes and every callback url and everything that it needs to redirect.
the main purpose of this route groups is to organize all the code.
the main purpose of moving the root file to the dashboard folder is because we use the brackets for dashboard it will not have any effect on the routes.
all the files added in the gitignore it will be automatically ignored from being committed to github.
it is important to write middleware in its correct letters as middleware is a reserved keyword in Nextjs.
usually by default the middleware protect the authenticated routes, but not with the new update, all routes are public by default, it is up to us to change the middlware configuration.
shadcn-ui comes preloaded with lucide-react when you choose default otherwise when you choose newyork it will come with radix icons.
creating API routes with HONO in nextjs.
the structure that is preferred is to create an api folder, instead of writing page.tsx we use route.ts, we use route handlers like GET, POST, PATCH and PUT.
if we need aditional routes we will have to create additional folder.
So basically we have to create an endpoint that is going to go through HONO instead of regular handlers and API folders will be used for that.
Working with HONO is really powerful as it allows RPC which means sharing of the API specifications between server and client. you can pass a bunch of middlewares when you working with HONO. Middlewares can be validators, permission protectors etc. 
I used GPT to give me the differences between HONO and Nextjs API routes and this is what it says so please note this down
  -->








Key differences between HONO and Nextjs API routes

  <!-- Using the Hono web framework versus Next.js API routes involves differences in design philosophy, performance, and intended use cases. Here are the key differences:

1. **Performance and Size**:
   - **Hono**: Known for being ultrafast and lightweight, with a minimal footprint (the "hono/tiny" preset is under 14kB) and zero dependencies. It uses the Web Standard API directly and optimizes performance by avoiding linear loops in its router (RegExpRouter)【7†source】【9†source】.
   - **Next.js API Routes**: While Next.js is also performant, it comes with more overhead due to its comprehensive features for building full-stack applications, including server-side rendering, static site generation, and client-side routing. This can result in a larger bundle size compared to Hono.

2. **Flexibility and Ecosystem**:
   - **Hono**: Designed to be extremely flexible, allowing developers to use it across multiple JavaScript runtimes (e.g., Cloudflare Workers, AWS Lambda, Node.js). It is suitable for edge computing scenarios where low latency and high performance are critical.
   - **Next.js**: Provides a robust set of tools and features for building React applications, including built-in support for API routes. It is ideal for projects that benefit from a full-featured React framework with integrated SSR and static site generation capabilities.

3. **Development Experience**:
   - **Hono**: Offers a clean and minimalistic API, with first-class TypeScript support, making it developer-friendly for those who prefer working close to the web standards with minimal abstractions【7†source】【9†source】.
   - **Next.js**: Provides a more extensive development environment with built-in routing, data fetching methods (getStaticProps, getServerSideProps), and various plugins and integrations that streamline the development of complex web applications【7†source】【9†source】.

4. **Use Cases**:
   - **Hono**: Best suited for performance-critical applications deployed at the edge, microservices, or scenarios where minimal overhead is crucial. Its lightweight nature makes it ideal for serverless and edge computing environments【7†source】【9†source】.
   - **Next.js**: Ideal for building full-stack React applications with dynamic routing, SSR, SSG, and API endpoints. It’s great for projects that require a comprehensive framework with extensive features and an ecosystem designed for React【7†source】【9†source】.

In summary, if you need a high-performance, lightweight solution for edge computing or microservices, Hono might be a better fit. For full-stack React applications with built-in API routes and comprehensive features, Next.js is likely the better choice. -->