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

React Router is a library used to manage navigation in single-page React applications (SPA). Instead of reloading the entire page when a user navigates between views, React Router enables the app to dynamically update the view by only changing certain parts of the UI, which keeps the user experience smooth and fast. 
Import React Router Components
Wrap Your App with BrowserRouter
Define Routes Using Routes and Route
Use Link or NavLink for Navigation:

The <Routes> component is a container that holds all the individual routes (<Route> components). It manages the rendering of different components based on the current URL. The key role of <Routes> is to ensure that only one matching route is rendered at any given time.

	•	Routing Context: It acts as the routing context, allowing the app to “listen” to changes in the browser’s address bar and determine which route should be rendered.
	•	Exclusive Route Matching: Only the first matching route inside the <Routes> container is rendered. This ensures that when a path matches, only the associated component is shown, preventing multiple components from being displayed accidentally.

The <Route> component defines an individual route, mapping a URL path to a React component. It consists of two main props:

	•	path: This defines the URL segment that will trigger the route to render.
	•	element: This specifies the React component that will be rendered when the path matches the current URL.

Each <Route> is a mapping of a specific URL path to the corresponding component.

Question 2

Nested routes
- nesting pieces of url
- shared UI
- -shared user interfaces
- want to keep same UI and display more