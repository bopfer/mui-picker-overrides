This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## To reproduce error

1. Clone this repository
2. Run `yarn` to install dependencies.
3. Run `yarn type-check` to show the following error:

   ```text
   node_modules/@material-ui/core/styles/overrides.d.ts:100:64 - error TS2344: Type 'ComponentNameToClassKey[Name]' does not satisfy the constraint 'string'.
     Type '"fixed" | "required" | "square" | "active" | "disabled" | "track" | "default" | "error" | "progress" | "message" | "middle" | "media" | "hidden" | "body" | "button" | "caption" | ... 486 more ... | undefined' is not assignable to type 'string'.
       Type 'undefined' is not assignable to type 'string'.

   100   [Name in keyof ComponentNameToClassKey]?: Partial<StyleRules<ComponentNameToClassKey[Name]>>;
                                                                   ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   ```
