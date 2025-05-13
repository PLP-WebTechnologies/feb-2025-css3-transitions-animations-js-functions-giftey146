# CSS3 Transitions, Animations, and Advanced JavaScript Functions

## Objectives

Create smooth CSS transitions and animations.
Use JavaScript functions for dynamic behavior.
Implement local storage for data persistence.

## Instructions
Add CSS animations to elements like buttons or images.

>[!NOTE]
> - Write a JavaScript function that:
> - Stores and retrieves user preferences using localStorage.
> - Implements an animation triggered by user actions.

## Tasks

Create a CSS animation.
Store data in localStorage.
Apply JavaScript to trigger animations.
// Apply animation on button click
document.getElementById("animateBtn").addEventListener("click", function() {
    this.classList.toggle("animated");
});

// Store user preference in localStorage
function savePreference(key, value) {
    localStorage.setItem(key, value);
}

function getPreference(key) {
    return localStorage.getItem(key);
}

// Example usage
document.getElementById("themeSwitch").addEventListener("change", function() {
    savePreference("theme", this.checked ? "dark" : "light");
    alert("Theme preference saved!");
});

button {
    background-color: blue;
    color: white;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    transition: background-color 0.5s ease-in-out;
}

button:hover {
    background-color: red;
}

@keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
}

.animated {
    animation: bounce 0.6s infinite;
}


Happy Coding! 💻✨
