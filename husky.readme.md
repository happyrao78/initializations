npm init -y
npm install --save-dev prettier
npm install husky --save-dev
npx husky init
npm install --save-dev lint-staged
<>
add this in pre commit hook
npx lint-staged
</>
{
  "lint-staged": {
    "client/**/*.{js,jsx,ts,tsx}": ["npx prettier --write"],
    "admin/**/*.{js,jsx,ts,tsx}": ["npx prettier --write"],
    "server/**/*.{js,ts}": ["npx prettier --write"]
  }
}
