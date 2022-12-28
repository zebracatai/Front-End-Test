# Implement Customizable, Fast And Well-Performanced Table Implementation With ReactJS

> You Should Implement a Library with React for React Applications, This Lib responsible for implement Tabel 



### React--Table library Usage
```jsx

import ReactTable from '..'

const config: IConfig =
{
    data: IData; // Data filled in table
    columns: IColumn[]; // Generate columns
    options?: IOptions; // Table configurations like table style
};

<ReactTable config={config} />



```



**data** (required)

```ts
const data: CTData = [
    ["cell 1", "cell 2", "cell 3"], // row 1
    ["cell 1", "cell 2", "cell 3"] // row 2
];
```


**columns** (required)

```ts
const columns: CTColumns = [
    {title: "Column 1"},
    {title: "Column 2", options: { textAlign: "center" }},
    {
        title: "Column 3",
        options: {
            textAlign: "right", 
            fontSize: 14,
            fontWeight: "bold",
            fontFamily: "serif",
            color: "#444444",
            lineHeight: 1
    	}
    }
];
```

**options** (optional)

```ts
const options: CTOptions = {
    borders: {
        column: undefined,
        header: undefined,
        row: { width: 1, color: "#555" },
        table: { width: 2, color: "#aaa" }
    }
}
```

*defaultOptions*

```ts
const defaultOptions: CTInternalOptions = {
    borders: {
        header: { color: "#ccc", width: 1 }
    },
    header: {
        fontSize: 12,
        fontWeight: "bold",
        fontFamily: "sans-serif",
        color: "#666666",
        lineHeight: 1.2,
        textAlign: "left",
        padding: 5
    },
    cell: {
        fontSize: 12,
        fontWeight: "normal",
        fontFamily: "sans-serif",
        color: "#444444",
        lineHeight: 1.2,
        padding: 5,
        textAlign: "left"
    },
    background: "#ffffff",
    devicePixelRatio: 2,
    padding: {
        bottom: 20,
        left: 20,
        right: 20,
        top: 20
    },
    subtitle: {
        fontSize: 14,
        fontWeight: "normal",
        fontFamily: "sans-serif",
        color: "#888888",
        lineHeight: 1,
        textAlign: "center"
    },
    title: {
        fontSize: 14,
        fontWeight: "bold",
        fontFamily: "sans-serif",
        color: "#666666",
        lineHeight: 1,
        textAlign: "center"
    }
};
```
_________________

### Please Get Fork From This Repo And Share Your Repo With Us
_________________

> **Requirement Task**

1. Implement app with Webpack from scratch
2. Implement Project with TypeScript
3. Dont use any UI Framework or lib module 
4. Implement Unit Test for Components
5. Consider This project as Scalable Project in futures and use any tools and tip needed for build maintainable and Scalable project
6. Consider best practice for your commit

> **Advanced Tasks**

1. Each cell should be selectable and pass selected cell (Important Bounes)
2. consider accessible ( screenreader-friendly )
3. passing performance tests with high grades [PageSpeed || YSlow || Chrome Dev Tools Audit]


### Define `/example` folder in root and implement `<ReactTable />` component with custom configurations ( custom props )

