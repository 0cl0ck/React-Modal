
# React Modal Component

A lightweight, customizable modal component for React applications.

## Installation

To install the component, use npm:

```bash
npm install @hughsawed/react-modal-component
```

## Usage

Here's a basic example of how to use the modal component:

```jsx
import React, { useState } from "react";
import Modal from "@hughsawed/react-modal-component";

function App() {
  const [isOpen, setIsOpen] = useState(false);

  return (
    <div>
      <button onClick={() => setIsOpen(true)}>Open Modal</button>
      <Modal isOpen={isOpen} onClose={() => setIsOpen(false)}>
        <h2>Modal Content</h2>
        <p>This is the content of the modal.</p>
      </Modal>
    </div>
  );
}
```

## Props

The component accepts the following props:

| Prop     | Type     | Default  | Description                                  |
| -------- | -------- | -------- | -------------------------------------------- |
| `isOpen` | boolean  | required | Controls the visibility of the modal.        |
| `onClose`| function | required | Function to call when the modal should close.|
| `children`| node    | required | Content to be rendered inside the modal.     |

## Features

- **Lightweight** and easy to use.
- **Customizable** content.
- Manages **body scroll** when the modal is open.
- **Accessible**, with appropriate ARIA attributes.
- Closes on outside click.


## Development

To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/react-modal-component.git
   ```
2. Navigate to the project directory:
   ```bash
   cd react-modal-component
   ```
3. Install the dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm start
   ```

## Contributing

Contributions are welcome! If you have any improvements or fixes, feel free to submit a pull request.

## License

This project is licensed under the MIT License.

