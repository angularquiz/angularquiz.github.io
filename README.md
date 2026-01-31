# Angular Quiz

A comprehensive, interactive quiz application to test and improve your Angular framework knowledge. Built as a single-page HTML application with no external dependencies.

**Live Demo:** [https://angularquiz.github.io](https://angularquiz.github.io)

## Overview

Angular Quiz features 200 carefully crafted questions spanning 20 different Angular topics. Each question presents 5 randomly selected options from a pool of 7 possible answers, ensuring a unique experience every time you take the quiz.

## Features

### Comprehensive Question Bank

- **200 questions** covering all major Angular concepts
- **20 categories** from basics to advanced topics
- **Two difficulty levels** - Easy and Medium
- **Detailed explanations** for every question

### Categories Covered

| Category | Topics |
|----------|--------|
| Components | Component creation, decorators, encapsulation, ViewChild |
| Templates & Data Binding | Interpolation, property binding, event binding, two-way binding |
| Directives | Structural directives, attribute directives, custom directives |
| Pipes | Built-in pipes, custom pipes, pure vs impure pipes |
| Services & DI | Injectable services, dependency injection, providers |
| Routing & Navigation | Router configuration, guards, lazy loading, parameters |
| Template-Driven Forms | ngModel, form validation, form state |
| Reactive Forms | FormControl, FormGroup, FormArray, validators |
| HTTP Client | HttpClient, interceptors, error handling |
| Observables & RxJS | Subjects, operators, subscriptions |
| Lifecycle Hooks | ngOnInit, ngOnDestroy, ngOnChanges, and more |
| Modules | NgModule, feature modules, shared modules |
| Angular CLI | Commands, configuration, schematics |
| Testing | Jasmine, Karma, TestBed, component testing |
| Change Detection | Strategies, Zone.js, ChangeDetectorRef |
| Decorators | @Input, @Output, @HostBinding, @HostListener |
| Signals | Signal creation, computed signals, effects |
| Standalone Components | Standalone APIs, bootstrapping, imports |
| Performance | Optimization techniques, lazy loading, tree-shaking |
| Security | XSS prevention, sanitization, CSRF protection |

### Customizable Quiz Settings

- **Category Selection** - Focus on specific topics or mix all categories
- **Difficulty Filter** - Choose Easy, Medium, or both
- **Question Count** - Select 10, 20, 50, 100, or all 200 questions
- **Timer Options** - No timer, 15, 30, 45, or 60 seconds per question

### Smart Randomization

Each question has 7 possible answer options, but only 5 are displayed per attempt. This means:
- The correct answer is always included
- 4 random incorrect options are selected
- Options are shuffled for each question
- Retaking the quiz provides a fresh experience

### Progress Management

- **Auto-Save** - Progress is automatically saved to browser storage
- **Resume Quiz** - Continue an unfinished quiz anytime
- **Settings Persistence** - Your preferences are remembered

### Timer System

- Visual countdown display
- Warning indicators (yellow at 10 seconds, red at 5 seconds)
- Pulsing animation for urgency
- Elapsed time tracking when timer is disabled
- Graceful handling when time expires

### Detailed Results

- Overall score percentage with visual indicator
- Correct and incorrect answer counts
- Total time taken
- Score breakdown by category with progress bars
- Performance-based feedback messages

### User Experience

- Clean, Angular-themed design
- Fully responsive for all devices
- Smooth animations and transitions
- Immediate feedback on answer selection
- Educational explanations after each question
- Option to quit and save progress

## Usage

### Starting a Quiz

1. Open the application in your web browser
2. Configure your quiz settings:
   - Select a category or choose "All Categories"
   - Choose difficulty level
   - Set the number of questions
   - Configure timer (optional)
3. Click "Start Quiz"

### Taking the Quiz

1. Read the question carefully
2. Select one of the five answer options
3. Review the explanation provided
4. Click "Next Question" to continue
5. Use "Quit Quiz" to save progress and exit

### Reviewing Results

After completing the quiz, you'll see:
- Your overall score percentage
- Number of correct and incorrect answers
- Time taken to complete
- Performance breakdown by category
- Option to retry or return to menu

### Resuming a Quiz

If you have an unfinished quiz:
1. A banner will appear on the start screen
2. Click "Resume" to continue where you left off
3. Click "Start New" to begin a fresh quiz

## Technical Details

### Architecture

- Single HTML file with embedded CSS and JavaScript
- No external dependencies or frameworks required
- No build process needed
- Works offline after initial load

### Data Storage

The application uses browser localStorage to persist:
- Quiz settings and preferences
- In-progress quiz state
- Answer history for resumption

### Scoring System

- Each correct answer: +1 point
- Each incorrect answer: 0 points
- Timed-out questions: Counted as incorrect
- Final score: (Correct / Total) × 100%

## Installation

### Option 1: Direct Use

Simply visit [https://angularquiz.github.io](https://angularquiz.github.io)

### Option 2: Local Hosting

1. Clone the repository:
```bash
git clone https://github.com/angularquiz/angularquiz.github.io.git
```

2. Open `index.html` in any web browser

### Option 3: Self-Hosting

1. Download the `index.html` file
2. Host on any static file server
3. No server-side processing required

## Contributing

Contributions are welcome! Here's how you can help:

### Adding Questions

Questions follow this structure:
```javascript
{
    question: "Your question text here?",
    options: ["Option 1", "Option 2", "Option 3", "Option 4", "Option 5", "Option 6", "Option 7"],
    correct: 0, // Index of correct answer (0-6)
    explanation: "Explanation of why this answer is correct.",
    difficulty: "easy" // or "medium"
}
```

### Guidelines

- Ensure questions are accurate and up-to-date
- Provide clear, educational explanations
- Include exactly 7 options per question
- Mark difficulty appropriately
- Test thoroughly before submitting

## License

MIT License

## Acknowledgments

- Built for the Angular developer community
- Inspired by the official Angular documentation
- Designed to support continuous learning

---

**Happy Learning!** 🅰️

Test your Angular knowledge and become an Angular expert!
