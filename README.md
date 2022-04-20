# React useStorage() hook

## Reeact Example Usage

```tsx
import { useStorage } from 'react-use-storage-hook';

function App() {
  // Similar to useState but first arg is key to the value in local storage.
  const [name, setName] = useStorage<string>("name", "Bob");

  return (
    <div>
      <input
        type="text"
        placeholder="Enter your name"
        value={name}
        onChange={(e) => setName(e.target.value)}
      />
    </div>
  );
}
```

Our own implementation of useStorage Hook, inspired by <https://usehooks.com/useLocalStorage>
We will modify some things in a close future.
