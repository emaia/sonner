[Sonner](https://github.com/emaia/sonner) is an opinionated toast component for React and Vanilla. Fork from [sonner](https://github.com/emilkowalski/sonner)

## Usage

To start using the library, install it in your project:

```bash
npm install @emaia/sonner
```

### Vanilla

```js

import { createToaster, toast } from 'sonner/vanilla';

const toaster = createToaster({
  position: 'bottom-right',
  theme: 'system',
  richColors: true,
  closeButton: true,
  expand: false,
  duration: 4000,
  gap: 14,
  visibleToasts: 3,
});

// Use toasts
toast('Hello World!');
toast.success('Operation successful!');
toast.error('Something went wrong!');
toast.info('Did you know?');
toast.warning('Be careful!');
toast.loading('Loading...');

```

### React

Add `<Toaster />` to your app, it will be the place where all your toasts will be rendered.
After that you can use `toast()` from anywhere in your app.

```jsx
import { Toaster, toast } from 'sonner';

// ...

function App() {
  return (
    <div>
      <Toaster />
      <button onClick={() => toast('My first toast')}>Give me a toast</button>
    </div>
  );
}
```

## Documentation

Find the full API reference in the [documentation](https://github.com/emaia/sonner).
