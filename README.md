# DJS08 Project Brief: React Router 

🎥 INSERT LOOM PRESENTATION LINK: [Here]

After cloning the repo, run `npm install` to install the dependencies 

Are you ready to get stuck into some React Router? For this challenge, you are required to code along with the lecturer from this lesson on Scrimba V1 [VanLife Project Bootstrapping](https://v1.scrimba.com/learn/react/introduction-to-react-router-6-coafa4877a450245212825034) or on Scrimba V2 click the link here [VanLife Project Bootstrapping](https://v2.scrimba.com/advanced-react-c02h/~02d)

The starter code has all the CSS styling required for the project; you will just need to link the corresponding classes as you code along. Jump into the start code here: [GitHub Repository](https://github.com/CodeSpace-Academy/StudentNo_Classcode_Group_Name-Surname_DJS08/tree/main).

The focus for this project will be to understand routing and present your code. Along with your code, you will need to submit a recorded presentation talking through the presentation points included below.

## React Routing Presentation Talking Points

For your recorded presentation, you will be discussing key concepts related to React Router, an essential tool for building single-page applications. To illustrate your understanding, address the following three questions in your presentation. These questions are designed to test your knowledge of the content from the "Advanced React Routing" Van Life Project, including setup, functionality, and application of React Router.

### Question 1: Explain the Setup and Basic Configuration of React Router

**Key Points to Cover:**
- What is the purpose of using React Router in a React application?
- How do you set up React Router using `BrowserRouter` as shown in the lessons?
- Describe the role of the `<Routes>` and `<Route>` components in defining the navigation structure.

### Question 2: Application of Route Parameters and Nested Routes

**Key Points to Cover:**
- Explain what route parameters are and how they are used in React Router, including the use of `useParams()` to access these parameters.
- Discuss the concept of nested routes as introduced in the lessons. What are nested routes, and how do they benefit the structure of a React application?
- Provide an example, such as the configuration for nested routes in the VanLife project.

### Question 3: Implementation of Navigation Controls and Dynamic Linking

**Key Points to Cover:**
- How does the `<Link>` component enhance navigation within a React application?
- Describe the use of `NavLink` for active styling. What makes `NavLink` different from the basic `Link` component?
- Discuss the use of search parameters and the `useSearchParams` hook to dynamically filter content, as seen in the VanLife project challenges.

Be prepared to provide code snippets and real-world application examples from your Van Life Project to support your explanations.

Make sure to submit your project to the DJS08 Project Tab on the LMS. Include a link to your Loom Presentation in your README.







Question 1  What is the purpose of using React Router in a React application?

React Router is a library used to manage navigation in single-page React applications (SPA). 
Instead of reloading the entire page when a user navigates between views, React Router enables the app to dynamically update the view by only changing certain parts of the UI, which keeps the user experience smooth and fast. 



Question 2   How do you set up React Router using BrowserRouter as shown in the lessons?

Import React Router Components
Wrap Your App with BrowserRouter
Define Routes Using Routes and Route

Question 3 

The <Routes> component is a container that holds all the individual routes (<Route> components). It manages the rendering of different components based on the current URL. The key role of <Routes> is to ensure that only one matching route is rendered at any given time.

	•	Routing Context: It acts as the routing context, allowing the app to “listen” to changes in the browser’s address bar and determine which route should be rendered.
	•	Exclusive Route Matching: Only the first matching route inside the <Routes> container is rendered. This ensures that when a path matches, only the associated component is shown, preventing multiple components from being displayed accidentally.

The <Route> component defines an individual route, mapping a URL path to a React component. It consists of two main props:

	•	path: This defines the URL segment that will trigger the route to render.
	•	element: This specifies the React component that will be rendered when the path matches the current URL.

Each <Route> is a mapping of a specific URL path to the corresponding component.



Question 4 Explain what route parameters are and how they are used in React Router, including the use of useParams() to access these parameters


Route parameters are used to define parts of the URL that are dynamic. For example, if you’re building a blog, you might have a URL structure where the post ID is part of the URL:
Defining Routes with Parameters:
You define a route parameter in a Route component using a colon (:) followed by the parameter name. For example:
To access the values of the route parameters in the component that is rendered by the route, you use the useParams hook provided by React Router.
In the component rendered by the route, you use the useParams() hook from react-router-dom to access the values of the parameters.


Question 5 & 6 Nested routes
- nesting pieces of url
- shared UI
- -shared user interfaces
- want to keep same UI and display more
- -header footer outlet in layout file 


Question 7 How does the <Link> component enhance navigation within a React application?


The <Link> component facilitates client-side navigation by preventing the browser from performing a full-page reload when navigating to a different route. This enhances performance and provides a smoother, faster user experience because the application does not have to reload the entire HTML page or re-fetch all resources from the server. Only the parts of the page that need to be updated (such as content or components) are changed.

Preserving Application State:

Since the <Link> component doesn’t trigger a full-page reload, application state (data held in React components or global state management like Redux) is preserved across different pages. This prevents unnecessary loss of user input or data that might happen with traditional anchor (<a>) tags, which cause the browser to reset the app state.


Question 8 Describe the use of NavLink for active styling. What makes NavLink different from the basic Link component?

Key Differences Between <NavLink> and <Link>:

	1.	Active Styling:
	•	NavLink allows you to apply specific CSS classes or styles to a link when it is “active”—i.e., when the route it links to matches the current URL.
	•	Link, on the other hand, is a simpler component that only provides navigation without offering active styling functionality.
	2.	Automatic Active Class:
	•	By default, <NavLink> automatically applies a CSS class called active to the link when the current URL matches the to prop.
	3.	Customization of Active Styles:
	•	You can customize the active styles by providing your own class or inline style through the className or style props using a function that checks whether the link is active.

Question 9 Discuss the use of search parameters and the useSearchParams hook to dynamically filter content, as seen in the VanLife project challenges.

n React Router, search parameters (also known as query parameters) are key-value pairs appended to the end of a URL that provide additional context or information for the request. The useSearchParams hook allows you to read and manipulate these search parameters to dynamically filter content in your application. This functionality is especially useful in scenarios like filtering lists or managing user search queries, as demonstrated in projects like the VanLife challenge where users filter van rentals by criteria such as price, type, or availability./vans?type=camper&price=low