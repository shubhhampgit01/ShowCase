
# 1 Quiz App with Stepper Proof of Concept

This repository contains a proof of concept (POC) implementation of a quiz app with a stepper. The app allows users to progress through a series of questions, with a stepper indicating their current position in the quiz. This POC demonstrates the use of stepper components in web applications for guiding users through multi-step processes.



## Features

- **Quiz Interface**: Provides a user-friendly interface for answering quiz questions.
- **Stepper Navigation**: Utilizes a stepper component to indicate the user's progress and navigate between quiz steps.
- **Responsive Design**: Ensures a seamless experience across various screen sizes and devices.



## Demo

A live demo of the quiz app with stepper POC is available https://quiz-app-mu-ruddy.vercel.app


## GitHub repository

GitHub repository link : https://github.com/shubhhampgit01/POC-quiz-app


# 2 Draggable Boxes POC

This repository contains a web application that allows users to interact with draggable boxes on the screen. Users can drag boxes around the screen and place them in any desired location. Additionally, users have the option to create custom boxes with their preferred dimensions and styling. This app provides a simple yet interactive way for users to manipulate and arrange boxes on the screen.
## Features

- **Draggable Boxes**: Enables users to drag boxes across the screen using mouse or touch input.
- **Custom Box Creation**: Allows users to create custom boxes with specified dimensions, colors, and styles.
- **Dynamic Box Placement**: Boxes can be placed and rearranged anywhere on the screen, providing flexibility in layout customization.
## Demo

A live demo of the draggable boxes app is available here : https://draggable-box.web.app/
## GitHub repository

GitHub repository link : https://github.com/shubhhampgit01/POC-draggable-box-example?tab=readme-ov-file


# 3 Socket Chat App POC 

This repository contains a real-time chat application with a backend built using Node.js and a frontend developed with React. The app utilizes WebSocket technology for instant messaging between users, providing a seamless and interactive chatting experience. The user interface (UI) is designed to be intuitive and user-friendly, enhancing the overall chat experience.
## Features

- **Real-Time Messaging**: Enables instant messaging between users in real-time using WebSocket technology.
- **Node.js Backend**: Utilizes Node.js for the server-side implementation, facilitating efficient handling of chat messages and user connections.
- **React Frontend**: Implements the frontend using React, providing a dynamic and responsive user interface.
## GitHub repository

GitHub repository link : https://github.com/shubhhampgit01/POC-socket-chat


# 4 POC of PARALLAX EFFECT

This repository contains a proof of concept (POC) implementation of a parallax effect, showcasing a visually appealing design with smooth animation effects. The parallax effect is a technique where background elements move at a different speed than foreground elements, creating an illusion of depth and immersion as the user scrolls or interacts with the interface.
## Features

- **Parallax Scrolling**: Background elements scroll at a different speed compared to foreground elements, providing a sense of depth and dimension.
- **Smooth Animation Effects**: The transition and animation effects are carefully crafted to ensure a seamless and visually pleasing experience.
- **Customizable**: Easily customizable to fit various design themes and requirements.
- **Responsive Design**: The parallax effect is optimized for various screen sizes and devices, ensuring a consistent user experience across platforms.
## Demo

A live demo of the parallax effect POC is available here https://parallax-rks.netlify.app/
## GitHub repository 
GitHub repository link : https://github.com/shubhhampgit01/POC-parallax-effect


# 5 useCallBack and useMemo Overview

Welcome to the guide on useCallback and useMemo hooks in React! This document aims to provide a clear understanding of these concepts and their practical use cases in React applications
## What is useCallback and useMemo?

useCallback and useMemo are both hooks provided by React to optimize performance and manage state in functional components.
## useCallback

useCallback is a hook used to memoize functions. It returns a memoized version of the callback function that only changes if one of the dependencies has changed. This optimization is useful when passing callbacks to child components that rely on reference equality to prevent unnecessary renders.

## useMemo

useMemo is a hook used to memoize values. It memoizes the result of a function or computation and reuses the cached value until one of the dependencies changes. This optimization is helpful for expensive calculations or computations within a functional component.

## Why to use useMemo or useCallBack ?

Basically these hooks are used to improve performance of an app by preventing unnecessary re-renders , When a state value changes in a component, the entire component re-renders. However, sometimes functions within the component, which are not directly related to the changed state, also re-render unnecessarily which we dont want to do.

Consider a scenraio , you have a function whose values change rarely and it takes a considerable amount of time to execute and You may be passing this function to child components. Without using useCallback, whenever any other state value changes, this function will also re-render, causing the child components to render unnecessarily as well. This can lead to performance issues, especially in complex applications where many state variables are changing frequently, resulting in the re-rendering of the entire component each time.

So, To avoid this issue and prevent unnecessary re-renders of functions and child components, we utilize useCallback and useMemo effectively.

## GitHub repository

GitHub repository link : https://github.com/shubhhampgit01/hooks-example


# 6 Parallax Image Carousel Overview

The parallax image carousel is a user interface component that displays a series of images, allowing the user to scroll horizontally through them. The parallax effect adds depth and immersion to the carousel by moving the images at a different speed than the scrolling motion, creating a sense of perspective.

## Components Used
- **React Native**: A framework for building native applications using React.
- **Animated API**: Used to create animations with React Native.
- **Dimensions**: Retrieves the screen dimensions to set the size of carousel items.
- **Image and Text**: Standard React Native components for displaying images and text.
- **StyleSheet**: Used to create styles for React Native components.
## Features
- **Animated FlatList**: A horizontal scrolling list component from React Native that supports animation. This is used to render the carousel items.
- **Parallax Effect**: Achieved by using the Animated module to interpolate scroll position (scrollx) and translate the images horizontally (translateX).
- **Shadow and Styling**: Each carousel item is styled with a shadow effect (shadowColor, shadowOpacity, shadowRadius) and padding (padding: 12) to give a card-like appearance.
- **Avatar Image**: Positioned at the bottom-right of each carousel item, it displays a random avatar image fetched from the randomuser.me API.
- **Responsive Sizing**: Carousel item dimensions (ITEM_WIDTH and ITEM_HEIGHT) are calculated based on the screen dimensions.
## Implementation Details
- **Dimensions**: Retrieves the screen width and height, which are used to calculate the size of the carousel items (ITEM_WIDTH and ITEM_HEIGHT).
**Data**: An array of images and corresponding avatar URLs is prepared. Each item also includes a unique key for rendering purposes.
- **Animated Scroll**: The onScroll event is captured to animate the images based on the scroll position (scrollx).
- **Interpolation**: The scrollx value is interpolated to calculate translateX, which adjusts the position of the image in response to scrolling, creating the parallax effect.
### Conclusion
This parallax image carousel not only showcases a series of images but also demonstrates the use of animation and user interaction in React Native applications. It enhances user experience by providing a visually engaging and dynamic interface for exploring images.

This overview highlights the key aspects and functionality of the parallax image carousel implemented in the React Native application.

## GitHub repository

GitHub repository link : https://github.com/shubhhampgit01/POC-Parallax-Image-Carousel


# 7 Satck-Card-Animation

The stack card animation is a dynamic user interface component that showcases information cards in a stacked formation. It allows the user to navigate through the cards using swipe gestures, creating a smooth and visually appealing transition between each card.

## Components Used
- **React Native**: A framework for building native applications using React.
- **react-native-vector-icons**: Provides FontAwesome icons for use within the application.
- **react-native-reanimated**: A React Native library for creating animations.
- **react-native-gesture-handler**: Enables gesture recognition and touch handling in the application.
- **Dimensions**: Retrieves the dimensions of the screen.
- **StatusBar**: Hides the status bar for a more immersive experience.

## Features
1. **Gesture Handling**: Utilizes `GestureHandlerRootView`, `GestureDetector`, and `Gesture.Fling` from `react-native-gesture-handler` to detect swipe gestures (fling up and down).
2. **Animation with Reanimated**: Implements animations using `useSharedValue`, `withTiming`, `useAnimatedStyle`, `interpolate`, and `Extrapolation` from `react-native-reanimated` to create smooth transitions and scaling effects.
3. **Card Layout**: Each card (`Card` component) is positioned absolutely with a defined `zIndex` to create a stacked appearance. The cards also include detailed information such as type, time, distance, and role.
4. **Responsive Design**: The layout adjusts based on the device's screen dimensions (`Dimensions.get('window')`) and is responsive to changes in screen size.
5. **Styling**: Uses custom styles defined in the `StyleSheet.create` function to achieve a consistent and visually appealing design.

## Implementation Details
- **Gesture Handling**: Sets up fling gestures (`flingUp` and `flingDown`) to navigate through the cards. The `activeIndex` state manages which card is currently displayed.
- **Animated Styles**: `useAnimatedStyle` and interpolation functions animate the position (`translateY`) and scale of each card based on the `activeIndex`.
- **Card Component**: Displays detailed information (`type`, `from`, `to`, `distance`, `role`) along with an image (`locationImage`) for each card.
- **Background Color**: The primary background color (`colors.primary`) and light background color (`colors.light`) are defined for a consistent theme.

## Conclusion
This stack card animation provides an interactive and engaging user interface for navigating through information cards. It demonstrates the capabilities of React Native and its libraries (`react-native-reanimated` and `react-native-gesture-handler`) in creating smooth animations and gesture-driven interactions.

This overview summarizes the main features and functionality of the stack card animation implemented in the React Native application.

## GitHub repository
GitHub repository link : https://github.com/shubhhampgit01/POC-Satck-Card-Animation


# 8 Admin Dashboard with Chart.js

This repository contains the source code for an Admin Dashboard application built with React and Chart.js. The application provides a responsive and interactive interface for visualizing data through various types of charts and graphs.

## Features

### Dashboard
- **Summary Cards**: Display key metrics and statistics.
- **Charts and Graphs**: Interactive charts built using Chart.js, including line charts, bar charts, and pie charts.

### User Management
- **User List**: Display a list of users with details.
- **User Actions**: Ability to add, edit, and delete users.

### Data Visualization
- **Real-time Updates**: Charts that update in real-time based on data changes.
- **Customizable Views**: Ability to filter and customize the data displayed in charts.

### Responsive Design
- **Mobile-Friendly**: Fully responsive design that works well on both desktop and mobile devices.
- **Interactive UI**: Smooth and interactive user interface for better user experience.

## Technologies Used

### Frontend
- **React**: A JavaScript library for building user interfaces.
- **Chart.js**: A JavaScript library for creating beautiful and interactive charts.
- **React Chart.js 2**: A React wrapper for Chart.js.

### Styling
- **CSS**: Custom styling to ensure a modern and clean look.

### State Management
- **React Hooks**: Used for managing state and side effects.

## GitHub repository
GitHub repository link : https://github.com/shubhhampgit01/admin-dashboard-chartjs


# 9 Dashboard Chart.js Example

This repository contains a sample dashboard application built with React and Chart.js. The purpose of this project is to demonstrate how to create a responsive and interactive admin dashboard for visualizing data using various charts.

## Features

### Dashboard
- **Summary Widgets**: Display key metrics and insights.
- **Charts**: Various types of charts including line charts, bar charts, and pie charts created with Chart.js.

### Data Visualization
- **Dynamic Data**: Charts that update dynamically based on the data provided.
- **Interactive Charts**: Enable users to interact with the charts for better insights.

### Responsive Design
- **Mobile and Desktop Friendly**: The layout adjusts seamlessly to different screen sizes, ensuring usability on both mobile and desktop devices.
- **User-friendly Interface**: A clean and modern UI design for a better user experience.

## Technologies Used

### Frontend
- **React**: A JavaScript library for building component-based user interfaces.
- **Chart.js**: A versatile library for creating responsive and interactive charts.
- **React Chart.js 2**: A React wrapper for Chart.js, simplifying integration with React.

### Styling
- **CSS**: Custom styles to enhance the visual appeal of the dashboard.


## GitHub repository
GitHub repository link : https://github.com/shubhhampgit01/dashboard-chartjs-example


# 10 RealTimeChatApplication

The `realTimeChatApplication` repository is a real-time chat application designed to facilitate instant communication between users. It utilizes modern web technologies to provide a seamless and responsive messaging experience.

## Features

- *Real-time Messaging:* Enables users to send and receive messages instantly without refreshing the page.
- *User Authentication:* Secure authentication system to ensure only authorized users can access the application.
- *Message History:* Allows users to view previous messages when they log in, ensuring continuity in conversations.
- *Backend Server:* Includes a backend server that handles message storage, user authentication, and real-time communication using technologies like Socket.io.
- *Database Integration:* Uses a database (e.g., MongoDB) to store chat messages and user information securely.

## GitHub repository
GitHub repository link : https://github.com/shubhhampgit01/realTimeChatApplication
