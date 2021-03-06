## Breadcrumb
A generic breadcrumb component following the w3.org [breadcrumb](https://www.w3.org/TR/2017/NOTE-wai-aria-practices-1.1-20171214/examples/breadcrumb/index.html) pattern. The *breadcrumb* will accept any child elements but is built to work with `a` elements.

### Usage
To denote the current page the *breadcrumb* automatically sets the last child `aria-current` prop to "page", an enumerated type value for `aria-current`. Addtionally *breadcrumb* accepts an optional `separator` prop that will render a ReactNode between navigation elements.

### Accessibility
The *breadcrumb* component consists of a `nav` element with `aria-label` set to a `label` prop. One should set the `label` prop to identify the structure as a breadcrumb trail and make it a navigation landmark so that it is easy to locate. The last child element `aria-current` prop is marked "page" to indicate that it reprents the current page.