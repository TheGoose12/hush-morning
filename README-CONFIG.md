# Content Configuration Guide

## Overview
You can now edit all the app content by modifying the `content-config.json` file. No need to touch HTML or CSS - just update the JSON file and refresh the app!

## How to Edit Content

### 1. App Title & Branding
```json
"app": {
  "title": "Your November Journey",        // Main title on home screen
  "subtitle": "Coffee Membership Recap",   // Subtitle below title
  "audio": {
    "file": "demoHush.m4a",               // Audio file name
    "duration": "0:45"                     // Display duration
  },
  "userPhoto": "user-photo.jpg",          // User avatar in messages
  "vinylBackground": "record-bg.png",     // Vinyl record background
  "logo": "hush-logo-black.svg"          // App logo
}
```

### 2. Home Screen Messages
```json
"homeScreen": {
  "startButton": {
    "text": "Start Journey"                   // Start button text
  },
  "messages": [
    {
      "type": "text",
      "content": "Hey, this is an audio message from Adam and Ron."  // Text message content
    },
    {
      "type": "audio",
      "duration": "1:03"                  // Audio message duration display
    }
  ]
}
```

### 3. Coffee Sections
```json
"coffees": [
  {
    "id": "regular",                      // Internal ID (don't change)
    "label": "Regular",                   // Label shown on coffee
    "name": "Ethiopian Yirgacheffe",      // Coffee name
    "origin": "Yirgacheffe, Ethiopia",   // Origin text
    "originBrief": "Yirgacheffe, Ethiopia • Natural", // Brief origin shown on slide
    "notesBrief": "Fruity • Floral • Wine-like",      // Brief notes shown as tags
    "heroImage": "https://...",           // Main coffee image URL
    "backgroundImage": "assets/coffee-bg.jpg",        // Background image for slide
    "descriptors": ["fruity", "floral"], // Flavor descriptors
    "details": {
      "subtitle": "From the birthplace of coffee",  // Modal subtitle
      "description": "This exceptional coffee...",  // Description text
      "characteristics": {                // Key details
        "Processing": "Washed",
        "Altitude": "1,700-2,200m"
      },
      "story": "Grown by smallholder farmers..."     // Coffee story
    },
    "gallery": [                          // Slideshow images
      "https://image1.jpg",
      "https://image2.jpg"
    ]
  }
]
```

### 4. Community Spotlight
```json
"community": {
  "enabled": true,                     // Set to false to hide entire community section
  "title": "Community Spotlight",
  "member": {
    "name": "Whitney Chen",              // Member name
    "role": "Visual Storyteller",       // Member role
    "photo": "https://...",              // Member photo URL
    "description": "Documents coffee...", // Member description
    "stat": {
      "icon": "📸",                      // Stat icon
      "text": "Captured 200+ coffee stories"  // Stat text
    },
    "instagramButton": "View Instagram", // Button text
    "showcaseImage": "https://..."       // Featured work image
  }
}
```

### 5. Events Section
```json
"events": {
  "title": "November Highlights",        // Section title
  "subtitle": "Monthly Cupping Event",  // Section subtitle
  "gallery": [                          // Background slideshow images
    "https://image1.jpg",
    "https://image2.jpg"
  ],
  "stats": [                           // Bottom stats
    {
      "number": "24",
      "label": "Members"
    }
  ],
  "seeMoreButton": "See More",          // Button text
  "modal": {                            // Modal content when button clicked
    "title": "November Cupping Event",
    "subtitle": "Highlights from our monthly gathering",
    // ... more modal content
  }
}
```

### 6. Spotify Section
```json
"spotify": {
  "title": "Coffee Vibes",              // Playlist title
  "subtitle": "Your Monthly Playlist", // Playlist subtitle
  "embedUrl": "https://open.spotify.com/embed/...", // Spotify embed URL
  "playButton": "▶ Tap to Play Spotify" // Play button text
}
```

## Quick Tips

1. **Images**: You can use URLs (like Unsplash) or local file names (place files in the same folder)
2. **Text**: All text content can be changed - titles, descriptions, button labels, etc.
3. **Spotify**: Get embed URLs from Spotify's share options
4. **Backup**: Always backup your `content-config.json` before making changes
5. **Testing**: After editing, refresh the app to see changes

## Image Recommendations

- **Hero Images**: 1000x800px or larger
- **Gallery Images**: 800x600px 
- **User Photos**: 400x400px (square)
- **Member Photos**: 400x400px (square)

## Common Edits

- Change month: Update "November" to "December" throughout
- New coffee: Replace coffee names, origins, and images
- Different member: Update name, role, photo, and description
- New playlist: Update Spotify embed URL and titles

The app will automatically load your changes when refreshed!