# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.














<!-- slide dots Part Start   -->

<!-- .custom-dots .slick-dots li button{
  position: absolute;
  bottom: 30px;
  left: 0;
  border-radius: 50%;
  background-color: #7d7d7d;
  
  
}
.custom-dots .slick-dots li.slick-active button {
  background-color: red;
  border: 2px solid white;
} -->
<!-- slide dots Part End  -->



<!-- Next Arrows  -->

import React from 'react'
import { LuChevronRight } from "react-icons/lu";

const NextArrow = (props) => {
    const { onClick } = props;
  return (
      <LuChevronRight className='text-5xl text-deleteC cursor-pointer absolute top-1/2 -right-7 -translate-y-1/2 z-10' onClick={onClick}/>
  )
}

export default NextArrow