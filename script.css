// Sticky Header with Smooth Transition
window.onscroll = function() {stickyHeader()};

var header = document.querySelector('.header');
var sticky = header.offsetTop;

function stickyHeader() {
    if (window.pageYOffset > sticky) {
        header.classList.add("sticky");
    } else {
        header.classList.remove("sticky");
    }
}

// Form Validation with Cool Animation
const form = document.querySelector('form');
form.addEventListener('submit', function(event) {
    const name = form.querySelector('input[type="text"]');
    const email = form.querySelector('input[type="email"]');
    const message = form.querySelector('textarea');

    if (name.value === "" || email.value === "" || message.value === "") {
        event.preventDefault(); // Prevent form submission
        animateInvalidFields(name, email, message);
    } else {
        animateSuccess();
    }
});

function animateInvalidFields(name, email, message) {
    if (name.value === "") {
        name.classList.add("invalid");
        setTimeout(() => name.classList.remove("invalid"), 1000);
    }
    if (email.value === "") {
        email.classList.add("invalid");
        setTimeout(() => email.classList.remove("invalid"), 1000);
    }
    if (message.value === "") {
        message.classList.add("invalid");
        setTimeout(() => message.classList.remove("invalid"), 1000);
    }
}

// Success Animation after Form Submit
function animateSuccess() {
    form.reset();
    const successMessage = document.createElement('div');
    successMessage.innerHTML = "✅ Your message has been sent successfully!";
    successMessage.style.position = "fixed";
    successMessage.style.bottom = "20px";
    successMessage.style.left = "50%";
    successMessage.style.transform = "translateX(-50%)";
    successMessage.style.background = "#28a745";
    successMessage.style.color = "#fff";
    successMessage.style.padding = "1rem 2rem";
    successMessage.style.borderRadius = "0.5rem";
    successMessage.style.boxShadow = "0 0 15px rgba(0, 0, 0, 0.2)";
    successMessage.style.fontSize = "1.4rem";
    successMessage.style.opacity = "0";
    document.body.appendChild(successMessage);

    setTimeout(() => {
        successMessage.style.transition = "opacity 0.5s ease-in-out";
        successMessage.style.opacity = "1";
    }, 100);

    setTimeout(() => {
        successMessage.style.transition = "opacity 1s ease-out";
        successMessage.style.opacity = "0";
        setTimeout(() => successMessage.remove(), 1000);
    }, 3000);
}

// Scroll to Top Button with Animation
const scrollToTopButton = document.createElement("button");
scrollToTopButton.innerHTML = "↑";
scrollToTopButton.style.position = "fixed";
scrollToTopButton.style.bottom = "20px";
scrollToTopButton.style.right = "20px";
scrollToTopButton.style.padding = "1rem";
scrollToTopButton.style.fontSize = "1.5rem";
scrollToTopButton.style.backgroundColor = "#1DCD9F";
scrollToTopButton.style.color = "#fff";
scrollToTopButton.style.border = "none";
scrollToTopButton.style.borderRadius = "50%";
scrollToTopButton.style.cursor = "pointer";
scrollToTopButton.style.display = "none";
scrollToTopButton.style.transition = "transform 0.5s ease";
document.body.appendChild(scrollToTopButton);

window.onscroll = function() {
    if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
        scrollToTopButton.style.display = "block";
        setTimeout(() => {
            scrollToTopButton.style.transform = "scale(1.1)";
        }, 50);
    } else {
        scrollToTopButton.style.display = "none";
    }
};

// Scroll to top functionality with smooth scroll
scrollToTopButton.addEventListener("click", function() {
    window.scrollTo({ top: 0, behavior: "smooth" });
    scrollToTopButton.style.transform = "scale(1)";
});

// Animated Skill Bars (on Scroll)
const skills = document.querySelectorAll('.skills-box');
window.addEventListener('scroll', function() {
    skills.forEach(skill => {
        if (isInViewport(skill)) {
            skill.querySelector('.progress-bar').style.width = skill.getAttribute('data-progress');
        }
    });
});

function isInViewport(element) {
    const rect = element.getBoundingClientRect();
    return rect.top >= 0 && rect.left >= 0 && rect.bottom <= (window.innerHeight || document.documentElement.clientHeight);
}

// Interactive Navigation (Highlight on Hover)
const navLinks = document.querySelectorAll('.navbar a');
navLinks.forEach(link => {
    link.addEventListener('mouseenter', function() {
        link.style.transition = "transform 0.3s ease";
        link.style.transform = "scale(1.1)";
    });

    link.addEventListener('mouseleave', function() {
        link.style.transition = "transform 0.3s ease";
        link.style.transform = "scale(1)";
    });
});
