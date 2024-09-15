# Rocketship

 Rocketship is an experimental radix and shadcn inspired design system for Astro that provides a set of reusable components and styles to help you build faster and more consistent websites.

 Visit https://rocketship.run
 
 [!WARNING]
 This is an experiment. It is a work in progress. The components can change rapidly without notice. Please use with caution.
    


Rocketship is a free and open source set of Astro components that can be used in an Astro project. The components have the `.astro` extension and are meant to be used in the components directory in an Astro project. There is zero dependency, meaning that you don't need to install and use any external package.


### What can Rocketship do?

Rocketship comes with a set of components and theme files that can set the overall look and feel of a website. It can also manage light and dark modes of a website with relative ease. You can modify the color, border radius using Theme props that will be used by Rocketship components. You can also design your own components and use css variables to apply Themes. 

### How will this help my project?

Rocketship can drastically help reduce development times and help create a simple work flow to import and use components that can be reused endlessly. Using predefined colors and themes will make sure your project looks delightful by default, and easy to customize for your needs.



## How to use Rocketship components?

There is no installation required to use Rocketship in your Astro project. You can copy and paste the components in your Astro project.

Please remember that rocketship is still experimental and the components may change. 


### Step 1: Copy and paste the components to your project

To use rocketship components, you can copy the components from this github repo or rocketship.run website. 


### Step 2: Import the Theme.astro file in your Layout.astro file
The recommend way is to import the Theme.astro in your layout.astro file. 

For example, you Layout.astro file should look like this:

**Layout.astro**

```astro
---
import Theme  from '@components/Theme.astro'
---
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<Theme>
  <slot />
</Theme>

</body>
</html>
```

### Step 3: Add aliases to your tsconfig.json file

We also recommend to use aliases in your Astro project. 

For example, you can add the following to your tsconfig.json file:

**tsconfig.json**
```json
{
  "compilerOptions": {
    "paths": {
      "@components/*": ["./src/components/*"]
    }
  }
}
```

