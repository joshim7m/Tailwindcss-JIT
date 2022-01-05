npx tailwindcss -o ./build/style.css

# Start, create source file - src/style.css
# add directive to src/style.css
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

npx tailwindcss -i ./src/style.css -o ./build/style.css

# next, add just in time mode
  npx tailwind init

#configure the tailwind.config.js
  mode: 'jit',
  purge: './path/*.html',

npx tailwindcss -i ./src/style.css -o ./build/style.css --watch
