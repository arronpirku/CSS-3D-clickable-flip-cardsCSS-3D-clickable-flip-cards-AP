# CSS 3D Clickable Flip Cards  
Internship Assignment – Lime Light TechLead  

## Internship Task Overview

This project was developed as part of the Lime Light TechLead Internship Programme under the supervision of Egon and the team.

The objective of this task was to study, understand, and extend the provided CSS 3D clickable flip card example from the official repository:

https://github.com/Lime-Light-TechLead/CSS-3D-clickable-flip-cards

Interns were required to:

- Analyze the provided HTML structure  
- Work with the given SCSS styling  
- Understand the 3D transformation logic  
- Design and implement a creative, original version  
- Promote or advertise a product of choice  
- Deploy the project using GitHub Pages  

Deployment was mandatory for completion of the task.

**Deadline:** 20 FEB 2026  

---

## Project Description

This project presents a modern product showcase using 3D clickable flip cards built entirely with HTML and SCSS.

Each card displays:

- A visually styled product preview on the front  
- Detailed specifications on the back  
- Smooth 3D flip animation on click  
- No JavaScript interaction required  

The implementation focuses on clean layout, smooth transitions, and consistent card dimensions during flipping.

The final design promotes:

- Noise-Canceling Headphones  
- Smartwatch for Training  
- Cold Brew Coffee Kit  

---

## Technical Implementation

### Core Concepts Used

- CSS 3D transforms (`rotateY`)  
- Perspective and depth control  
- Backface visibility handling  
- SCSS nesting and variables  
- Flexbox layout system  
- Pure CSS interaction using checkbox toggles  

### Flip Mechanism

The card flip is controlled through a hidden checkbox input:

```scss
.more:checked ~ .content {
  transform: rotateY(180deg);
}
The .card container defines perspective:

.card {
  perspective: 1600px;
}
```
The front and back faces are layered using:

```scss
.front,
.back {
  position: absolute;
  inset: 0;
  backface-visibility: hidden;
}

.back {
  transform: rotateY(180deg);
}
```

## Design Approach

The design emphasizes:

- Visual depth using gradients and overlays  
- Clear typography hierarchy  
- Structured information layout  
- Consistent card dimensions  
- Clean spacing and alignment  
- Maintainable SCSS architecture  

Images are assigned via structured SCSS classes instead of inline styling to keep styling centralized and organized.

---

## Learning Outcomes

Through this task, the following skills were strengthened:

- Understanding CSS 3D rendering behavior  
- Structuring reusable UI components  
- Working with SCSS variables and nesting  
- Handling CSS state-based interactions  
- Maintaining clean and scalable code  
- Preparing projects for GitHub deployment  

---

## Author

Arron Pirku
