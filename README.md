<p align="center">
<img src="./public/img/logo.svg" alt="CryptoLister" width=70 />
</p>
<h3 align="center">CryptoLister</h3>

<p align="center">
<a href="https://nuxt.com/"><img src="https://img.shields.io/badge/Nuxt.js-%23ffffff.svg?style=for-the-badge&logo=nuxt.js&logoColor=00DC82" alt="Nuxt.js"></a>
<a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-%234FC08D.svg?style=for-the-badge&logo=vue.js&logoColor=white" alt="Vue.js"></a>
<a href="https://pinia.vuejs.org/"><img src="https://img.shields.io/badge/Pinia-%23ecb732.svg?style=for-the-badge" alt="Pinia"></a>
<a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-%233178C6.svg?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://img.shields.io/badge/JavaScript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"></a>
<a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-%23339933.svg?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js"></a>
<a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind_CSS-%2306B6D4.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS"></a>
<a href="https://vitejs.dev/"><img src="https://img.shields.io/badge/Vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"></a>
<a href="https://www.cypress.io/"><img src="https://img.shields.io/badge/Cypress.io-%2317202C.svg?style=for-the-badge&logo=cypress&logoColor=white" alt="Cypress.io"></a>
<a href="https://vitest.dev/"><img src="https://img.shields.io/badge/Vitest-%236E9F18.svg?style=for-the-badge&logo=vitest&logoColor=white" alt="Vitest"></a>
<a href="https://eslint.org/"><img src="https://img.shields.io/badge/ESLint-%234B32C3.svg?style=for-the-badge&logo=eslint&logoColor=white" alt="ESLint"></a>
<a href="https://prettier.io/"><img src="https://img.shields.io/badge/Prettier-%231A2B34.svg?style=for-the-badge&logo=prettier&logoColor=white" alt="Prettier"></a>
<a href="https://stylelint.io/"><img src="https://img.shields.io/badge/StyleLint-%236B3E99.svg?style=for-the-badge&logo=stylelint&logoColor=white" alt="StyleLint" /></a>
<a href="https://github.com/actions"><img src="https://img.shields.io/badge/GitHub-%23181717.svg?style=for-the-badge&logo=github&logoColor=white" alt="GitHib Actions" /></a>
</p>
<br />

# About

## Tasks to be done

### Installation
1. Clone this repository to your local machine.
2. Install the required dependencies by running `npm install`.
3. Start the development server by running `npm run dev`.
4. Open your browser and navigate to http://localhost:3000.

### Coding tasks
1. Go to the `CurrencyList.vue` component.
2. Show the value of the `filter` variable in the `div` `#filter-value`.
3. Implement the `isFilterActive` computed prop. - The computed prop `isFilterActive` should return `true` if the filter field is empty, otherwise `false`.
4. Make the contents of `#has-active-filter` to be dynamic: - Use the `isFilterActive` computed prop to conditionally render the contents of the `#has-active-filter` div.
5. Add a button to clear the filter in `#new-component`. - The button should clear the filter field when clicked. - `@click="clearFilter"`
6. Set the default value of the `filter` to be `bitcoin`
7. Allow the filtering of cryptocurrencies by symbol. - The computed prop `currencyListFiltered` should be filtered by `name` OR by `symbol`.
8. Extract the login from the `Set filter to ETH` to a method called `setFilterToETH`. - `@click="setFilterToETH"`
9. Make the filter case-insensitive. - The filter should be case-insensitive. - use `toLowerCase()` or `toUpperCase()`
10. The clear filter button should not be visible when the input field is not empty. Use the `v-if` directive to conditionally render the button.
11. Create new component `TuExercise.vue`. 
12. Put some text like `<span>Hello world</span>` and display the new component into the `CurrencyList.vue`
13. Move the logic from the `#new-component` div to the new component.
14. The new component should receive the `filterValue` prop.
15. The new component should emit an event `clear-filter` when the button is clicked.
16. The new component should emit an event `set-filter-to-eth` when the button is clicked.
17. Go to `CurrencyCard.vue` component.
18. Crete new computed prop `logoSrc` - The computed prop `logoSrc` should return the logo URL of the currency. Use the `symbol` property of the currency to generate the URL. - `/img/svg-crypto-logos/${symbol}.svg`. Use the new `logoSrc` computed prop to display the logo of the currency. `:src="logoSrc"`
19. Make the favorite button work. - The favorite button should toggle the favorite status of the currency. - Use the `toggleFavorite` method to toggle the favorite status of the currency. - `@click="toggleFavorite"`
20. Prevent the page from navigating when the favorite button is clicked. - Use the `prevent` and the `stop` modifiers to prevent the page from navigating when the favorite button is clicked. - `@click.stop.prevent="toggleFavorite"`
21. Make the favorite img to change src when the currency is favorite. - Use the `isFavorite` computed prop to change the src of the favorite img. - The url for the active state is `/img/heart-active.svg` and for the inactive state is `/img/heart-inactive.svg`
22. Extract the logic for the favorite buttn src into computed prop `favoriteSrc`.
23. Push the changes to a new github repository.

## Technologies Used

This project was built using the following technologies:

- **Nuxt.js**
- **Vue.js**
- **Pinia**
- **TypeScript**
- **JavaScript**
- **Node.js**
- **Tailwind**
- **Vite**
- **Cypress**
- **Vitest**
- **ESLint**
- **Prettier**
- **StyleLint**
- **CI/CD with GitHub Actions**

## Screenshots

Here are some screenshots of the project:

![Home](./screenshots/home.png)
![Home List](./screenshots/home-filter-no-data.png)
![Favorites](./screenshots/favorites.png)
![Overview](./screenshots/overview.png)
