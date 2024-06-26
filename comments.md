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
  -->