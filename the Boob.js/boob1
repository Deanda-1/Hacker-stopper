function checkForHackingActivities() {
  // Check if developer tools are open
  if (window.console && window.console.firebug) {
    console.log("Hacking detected: Developer tools are open.");
    // Optionally, perform some actions like logging the attempt or blocking access.
  }

  // Check if key combinations are used (right-click, F12, Ctrl+Shift+I, etc.)
  document.addEventListener("keydown", function (event) {
    if (
      event.keyCode === 123 ||
      (event.ctrlKey && event.shiftKey && event.keyCode === 73)
    ) {
      console.log("Hacking detected: Key combination used.");
      event.preventDefault(); // Prevent default action (e.g., opening developer tools on some browsers).
      // Optionally, perform some actions like logging the attempt or blocking access.
    }
  });

  // Check if the page is being loaded inside an iframe
  if (window.top !== window.self) {
    console.log("Hacking detected: Page is loaded inside an iframe.");
    // Optionally, perform some actions like logging the attempt or blocking access.
  }

  // Check if the right-click is disabled
  document.addEventListener("contextmenu", function (event) {
    event.preventDefault();
    console.log("Hacking detected: Right-click is disabled.");
    // Optionally, perform some actions like logging the attempt or blocking access.
  });
}
