# Modern Christmas Dinner Recipe Website

A collection of non-traditional Christmas dinner recipes with a modern, engaging style. The site features responsive design using Tailwind CSS and follows a consistent structure for easy content addition.

## Directory Structure

```
recipes/
├── index.html                      # Main landing page
├── collections/                    # Recipe collections
│   └── christmas-dinner-recipes.html
├── recipes/                        # Individual recipe pages
│   ├── pomegranate-maple-lamb-chops.html
│   ├── moroccan-stuffed-cornish-hens.html
│   └── [other-recipe-name].html
├── images/
│   ├── collections/               # Collection hero images
│   │   └── modern-christmas-dinner-recipe-collection.webp
│   └── recipes/                   # Recipe images
│       └── Pomegranate-Maple-Glazed-Lamb-Chops-recipe.webp
└── image.md                       # Image specifications and guidelines
```

## Adding New Content

### Adding a New Recipe

1. Create a new HTML file in the `recipes/` directory:
   - Use kebab-case for filenames: `your-recipe-name.html`
   - Copy the structure from an existing recipe file
   - Update metadata, title, and content

2. Add recipe images to `images/recipes/`:
   - Main recipe image: `Recipe-Name-recipe.webp`
   - Follow image specifications in `image.md`

3. Update the collection page:
   - Add a new recipe card in `collections/christmas-dinner-recipes.html`
   - Link to the new recipe page
   - Include the recipe image

### Image Guidelines

See `image.md` for detailed specifications, but in general:
- Hero Images: 1920x1080px (16:9)
- Recipe Cards: 800x600px (4:3)
- Process Images: 600x400px (3:2)
- Final Dish Images: 1200x800px (3:2)

## HTML Structure

### Collection Page Template
```html
<div class="bg-white rounded-lg shadow-md overflow-hidden">
    <div class="md:flex">
        <div class="md:w-1/3">
            <img src="../images/recipes/your-recipe-image.webp" alt="Recipe Name" class="w-full h-full object-cover">
        </div>
        <div class="p-6 md:w-2/3">
            <h3 class="text-2xl font-bold mb-2">[Number]. Recipe Name</h3>
            <p class="text-gray-600 mb-4">Brief, engaging description</p>
            <div class="flex flex-wrap gap-4 text-sm mb-4">
                <span class="bg-color-100 text-color-800 px-3 py-1 rounded-full">Prep time</span>
                <span class="bg-color-100 text-color-800 px-3 py-1 rounded-full">Cook time</span>
            </div>
            <a href="../recipes/your-recipe-name.html" class="inline-block bg-red-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-red-700 transition-colors">View Recipe</a>
        </div>
    </div>
</div>
```

### Recipe Page Sections
- Hero image with title and times
- Fun fact box
- Ingredients list
- Step-by-step instructions
- Process images
- Serving suggestions
- Storage tips
- Pro tips
- Make-ahead tips

## Style Guidelines

1. Writing Style:
   - Fun and engaging tone
   - Witty parentheticals
   - Casual but informative
   - Include fun facts and helpful tips

2. Visual Style:
   - Use Tailwind CSS classes
   - Consistent color schemes for different recipe types
   - Clear visual hierarchy
   - Responsive design for all screen sizes

## Development Notes

- The site uses Tailwind CSS via CDN
- All pages are responsive and mobile-first
- Images use the `object-cover` class for consistent sizing
- Navigation paths use relative links (`../`)
