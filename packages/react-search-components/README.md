# react-search-components

This is the view layers for react-search-ui.

This library provides view implementations for all of Search UI's components along with corresponding CSS, and a few layout components.

The components provided here have no logic behind them, they are simple, stateless,
view-only components.

## Usage

```jsx
import {
  Body,
  Header,
  Result,
  SearchBox
} from "@elastic/react-search-components";
import "@elastic/react-search-components/lib/styles/styles.css";

export default function App() {
  return (
    <div className="reference-ui">
      <Header>
        <SearchBox value="test" />
      </Header>
      <Body
        bodyHeader={
          <div class="meta">
            <PagingInfo
              end={10}
              searchTerm={"test"}
              start={1}
              totalResults={100}
            />
          </div>
        }
        bodyContent={
          <div>
            <Result title="A Result" />
          </div>
        }
      />
    </div>
  );
}
```

TODO: List all components here