# Showcase Components (React)

This is a small `React` component library to be used as containers for showcasing projects, portfolio work, guides etc that are better presented in the context of a phone or browser window.

For reference they look like this:

[![image](https://user-images.githubusercontent.com/13936670/54876204-0b01b900-4e60-11e9-967b-f005dd62032b.png)](https://alhinds.com/showcase-components)

## Configuring with Webpack
This package is meant to be used with a build tool to aid resolution of CSS modules. Webpack or similar with `style-loader` & `css-loader` will be required to use this package (although in most cases these packages should already be in use in most react build configurations).

## Reasoning
This entire package compressed is under 2K. An alternative `.png` type wrapper will be larger _and_ it won't be dynamic. Yay fast loading and customisation!

The API for the components is pretty simple.

## Example

```jsx
import React, { Component } from 'react'
import { Laptop } from 'showcase-components'

const MyAwesomePreview = (props) => (
    <Laptop>
        <iframe src={mywebsiteurl}></iframe>
    </Laptop>
)

// OR
const MyAwesomePreviewAsImg = (props) => (
    <Laptop>
        <img src={mywebsiteurl}></img>
    </Laptop>
)

// OR
const MyAwesomePreviewAsJsx = (props) => (
    <Laptop>
        <SomeOtherReactComponentsHere />
    </Laptop>
)
```

## Issues
Please feel free to lodge an issue at the public git repository.