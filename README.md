"# useRequestAnimationFrame-reack-hook"
Use the useRef() hook to create two variables. requestRef will hold the last request id and previousTimeRef will hold the last timestamp.
Define a function, animate, which handles updating these variables, runs the callback and calls Window.requestAnimationFrame() perpetually.
Use the useEffect() hook with an empty array to initialize the value of requestRef using Window.requestAnimationFrame(). Use the returned value and Window.cancelAnimationFrame() to clean up when the component unmounts.
