# ASSIGNMENT: ARCHITECTURE DECISION RECORD

## ADR: Development Approach for Food Ordering App

**Decision:** Hybrid App with React Native

**Context:** We're deciding how to build our app so it's efficient on both iOS and Android.

**Choice:** We've chosen to develop a hybrid app using React Native.

**Why?**
- React Native allows us to cover both platforms with one codebase, reaching a wider audience.
- It's known for providing a near-native user experience.
- React Native has a huge developer community and a wealth of libraries, which can speed up development.

**What to watch out for:**
- We may encounter some challenges in achieving native performance for complex animations or interactions.
- The team may need to adapt to React Native's development environment.
- Finding developers with specific React Native experience might initially be challenging.

**Next steps:**
- Provide React Native training for our development team.
- Focus on optimizing performance for both iOS and Android, especially in areas with complex user interactions.
- Regularly gather user feedback to make necessary adjustments for a seamless experience across platforms.

## ADR: UI Design and Framework with React Native for Food Ordering App

**Decision:** Utilizing React Native for UI Development

**Context:** For our app's interface, we need a framework that helps us create a user-friendly and visually appealing experience on both iOS and Android.

**Choice:** We've decided to use React Native for both app development and managing the UI.

**Why?**
- React Native is unique because it lets us write our app's UI with one codebase that works for both major mobile platforms.
- It offers a wide range of ready-to-use UI components that are designed to feel native on both iOS and Android.
- The framework is supported by a large community of developers, providing us with resources, libraries, and tools that make development faster and more efficient.

**What to watch out for:**
- While React Native aims for a native feel, there might be instances where achieving 100% native look or performance for highly custom interactions requires additional work.
- Our team may need to ramp up on React and React Native specifics, especially if they're more accustomed to other frameworks.

**Next steps:**
- Organize React Native training sessions for our developers to ensure everyone is up to speed.
- Dive into React Native's component library and select UI components that best fit our app's design requirements.
- Keep testing our app on both iOS and Android devices to ensure the UI feels natural and performs well, making adjustments as needed based on feedback.

## ADR: Backend Language for Food Ordering App

**Decision:** Use Node.js

**Context:** We need a strong system on the server side to handle orders and payments.

**Choice:** We're going with Node.js.

**Why?**
- It's great for handling many tasks at once, like processing orders.
- There's a big community of developers using Node.js, so we have lots of resources and support.
- It works well with the databases and payment systems we want to use.

**What to watch out for:**
- Our team might need some time to get used to writing server code in JavaScript.
- If we're doing a lot of complicated calculations, we need to plan carefully to keep things running fast.

**Next steps:**
- Train any team members who are new to Node.js.
- Use best practices to manage heavy-duty tasks without slowing down the app.

## ADR: Permissions Strategy for Food Ordering App

**Decision:** Just-In-Time Permissions Requests

**Context:** We need to ask users for permissions like their location, but we want to do it without making them uncomfortable.

**Choice:** Ask for permissions only when we need them, not all at once.

**Why?**
- People are more likely to say yes if they understand why we're asking.
- It shows we care about their privacy.
- It avoids overwhelming users right when they install the app.

**What to watch out for:**
- We need to plan carefully to make sure we ask at the right time.
- It might interrupt what the user is doing in the app.

**Next steps:**
- Design clear messages that explain why we need each permission.
- Watch how users react and adjust our approach if needed.

## ADR: Data Storage for Food Ordering App

**Decision:** Hybrid Storage with Firestore and SQLite

**Context:** Our app needs to store data like menu items and user orders. We want this to work fast and even when there's no internet.

**Choice:** Use Firestore for storing data online and SQLite for data on the user's device.

**Why?**
- Users can see up-to-date menus and track their orders in real-time with Firestore.
- With SQLite, they can still look at menus and their past orders even without internet.
- This mix lets us balance speed and availability.

**What to watch out for:**
- Syncing data between online and device storage can get complicated.
- We need to make sure the app doesn't use too much space on the user's device.

**Next steps:**
- Set up a system to keep online and device data matched up.
- Keep an eye on how much data we're storing on devices to avoid taking up too much space.

## ADR: Using Additional Frameworks or Technology Stacks

**Decision:** Integrate Selected External Services

**Context:** We want to add features like easy logins, notifications, and payments without building everything from scratch.

**Choice:** Use Firebase for things like logins and notifications, and Stripe for payments.

**Why?**
- Firebase offers a lot of features we can use right away, which saves time.
- Stripe is a safe and easy way for users to pay in the app.
- Both services are trusted and widely used, which can make our users feel more secure.

**What to watch out for:**
- Relying on these services means we have less control over these parts of our app.
- Costs can vary based on how much we use these services.

**Next steps:**
- Plan our app's architecture to make sure we can switch services later if we need to.
- Keep track of our usage to manage costs effectively.
