## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## my notes
By default, Next.js applications use React Server Components. https://nextjs.org/learn/dashboard-app/fetching-data

I am unclear about why it either loads dynamically or statically. Chapter 8-10
CH.10 Static vs. Dynamic Routes

For most web apps built today, you either choose between static and dynamic rendering for your entire application, or for a specific route. And in Next.js, if you call a dynamic function in a route (like querying your database), the entire route becomes dynamic.

is that "async function"

chat answer: 
    Regarding your question about static vs. dynamic rendering:
A route becomes dynamic when you use:
async functions that fetch data
Dynamic functions like cookies() or headers()
Dynamic route segments (like [id])
Search params or dynamic API calls
You can explicitly control this behavior using the dynamic route segment config option if needed.

TODO:
- research ways to build native apps
https://nextjs.org/learn/dashboard-app/mutating-data#6-revalidate-and-redirect
Since you're updating the data displayed in the invoices route, you want to clear this cache and trigger a new request to the server. You can do this with the revalidatePath function from Next.js:


not covered in the course:
https://nextjs.org/learn/dashboard-app/improving-accessibility
To maintain form values across re-renders, you should use controlled components with value and checked props instead. Here's how to fix it: