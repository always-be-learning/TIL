# :sparkles: TIL :sparkles:

Today we learned some stuff!

## How to contribute

1. Clone this repo
2. Create a branch for your newly-learned thing
3. Add your newly-learned thing as a Markdown (`.md`) file in a category folder   
 * e.g. `removing-glitter-polish.md` in the `beauty` category folder
4. You can open a pull-request if you like _or_ you can merge directly into `master` :scream:

   ```
   git checkout master 
   git pull origin master 
   git merge your-newly-learned-thing --ff
   git push origin HEAD
   ```
   
   **Notes:**
   * Checking out `master` again and getting latest to to avoid potential merge conflicts
   * I use `HEAD` when I'm pushing to avoid branch typos (yes, I know you can tab-complete, but I like this better; learned it from @tcopeland :two_hearts:)
