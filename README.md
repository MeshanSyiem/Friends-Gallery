# Friends Gallery

A beautiful, responsive photo and video sharing gallery application with a secure login system and modern glassmorphism design.

## 🌟 Features

### Core Functionality

- **Secure Login System**: Protected access with username/password authentication
- **Multi-Media Support**: Upload and display photos (JPG, PNG, GIF) and videos (MP4, MOV, AVI)
- **Responsive Masonry Gallery**: Pinterest-style layout that adapts to different screen sizes
- **Infinite Scroll**: Automatically loads more content as you scroll down
- **Drag & Drop Upload**: Easy file uploading with multiple file selection
- **Delete Functionality**: Remove unwanted items with confirmation dialog

### Visual Design

- **Glassmorphism UI**: Modern frosted glass aesthetic with backdrop blur effects
- **Smooth Animations**: Fade-in effects, hover transitions, and transform animations
- **Gradient Backgrounds**: Beautiful color gradients for visual appeal
- **Mobile Responsive**: Optimized for desktop, tablet, and mobile devices

### User Experience

- **Auto-Play Videos**: Videos play on hover and pause when mouse leaves
- **Performance Optimized**: Loads content progressively for better performance
- **Empty State**: Friendly messaging when no content is available
- **Visual Feedback**: Hover effects and button states for better interaction

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No server setup required - runs entirely in the browser

### Installation

1. Save the HTML file to your computer (e.g., `friends-gallery.html`)
1. Open the file in your web browser
1. You’re ready to go!

### Login Credentials

- **Username**: `CS`
- **Password**: `CS2022`

> ⚠️ **Security Note**: This is a demo application with hardcoded credentials. For production use, implement proper authentication with a backend server.

## 🎯 How to Use

### Logging In

1. Open the application in your browser
1. Enter the username: `CS`
1. Enter the password: `CS2022`
1. Click “Enter” to access the gallery

### Uploading Media

1. Click the “Choose Files” button in the upload section
1. Select one or multiple photos/videos from your device
1. Supported formats: JPG, PNG, GIF, MP4, MOV, AVI
1. Files will automatically appear in the gallery with smooth animations

### Managing Content

- **View Videos**: Hover over videos to auto-play, they’ll pause when you move away
- **Delete Items**: Hover over any item and click the red “×” button to delete
- **Scroll Loading**: Scroll down to automatically load more content (if you have many items)

## 📱 Browser Compatibility

### Fully Supported

- Chrome 88+
- Firefox 85+
- Safari 14+
- Edge 88+

### Features Used

- CSS Grid & Flexbox
- CSS Backdrop Filter (glassmorphism effect)
- File API for image/video uploads
- HTML5 Video with autoplay controls

## 🎨 Customization

### Changing Login Credentials

```javascript
// In the doLogin() function, modify these values:
if (u === 'YOUR_USERNAME' && p === 'YOUR_PASSWORD') {
```

### Adjusting Color Scheme

```css
/* Main gradient background */
body { 
  background: linear-gradient(135deg, #your-color1 0%, #your-color2 100%); 
}

/* Glass panel transparency */
.glass {
  background: rgba(255,255,255,0.6); /* Adjust opacity (0.6) */
}
```

### Modifying Upload Limits

```javascript
// Change items loaded per batch
const itemsPerLoad = 10; // Change this number
```

### Supported File Types

```html
<!-- Modify the accept attribute -->
<input type="file" accept="image/*,video/*,your-custom-types">
```

## 🔧 Technical Details

### Architecture

- **Frontend Only**: Pure HTML, CSS, and JavaScript
- **No Dependencies**: No external libraries or frameworks required
- **Local Storage**: Uses browser memory (not persistent between sessions)

### File Handling

- Uses FileReader API to convert files to Base64 data URLs
- Stores media in JavaScript arrays during session
- No server upload - everything runs client-side

### Performance Optimizations

- Lazy loading with infinite scroll
- CSS transforms for smooth animations
- Efficient DOM manipulation
- Masonry layout with CSS columns

### Responsive Breakpoints

```css
@media (max-width: 768px) {
  /* Mobile styles */
  .gallery { column-width: 200px; }
}
```

## 🛠️ Development

### File Structure

```
friends-gallery.html          # Main application file
├── HTML structure           # Login page + app layout
├── CSS styles              # Glassmorphism design + responsive layout
└── JavaScript logic        # Authentication + file handling + gallery management
```

### Key Functions

- `doLogin()`: Handles user authentication
- `renderGallery()`: Updates the visual gallery display
- `loadMore()`: Implements infinite scroll loading
- `deleteItem(id)`: Removes items from gallery

## 🚨 Limitations & Considerations

### Security

- **Demo Purpose Only**: Hardcoded credentials are not secure
- **Client-Side Only**: No server-side validation or storage
- **No Data Persistence**: Uploaded files are lost when page refreshes

### File Size

- Large files may cause browser performance issues
- No file size limits implemented
- All files stored in browser memory

### Browser Storage

- Does not use localStorage/sessionStorage
- Content is temporary and session-based only

## 🔮 Future Enhancements

### Potential Improvements

- Backend integration with proper authentication
- Database storage for persistent media
- User accounts and sharing capabilities
- File compression and optimization
- Thumbnail generation for better performance
- Social features (comments, likes, sharing)
- Admin panel for user management
- Progressive Web App (PWA) capabilities

### Advanced Features

- Face recognition and tagging
- Automatic photo organization by date/location
- Bulk operations (select multiple, batch delete)
- Photo editing capabilities
- Cloud storage integration
- Real-time collaboration

## 🐛 Troubleshooting

### Common Issues

**Login not working**

- Ensure username is exactly `CS` (case-sensitive)
- Ensure password is exactly `CS2022`
- Try refreshing the page

**Files not uploading**

- Check if file format is supported
- Try with smaller file sizes
- Ensure browser supports File API

**Videos not playing**

- Check browser video codec support
- Try converting to MP4 format
- Ensure video file isn’t corrupted

**Layout issues on mobile**

- Clear browser cache
- Try rotating device orientation
- Update to latest browser version

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

This is a demo application, but feel free to:

- Fork and modify for your own use
- Report bugs or suggest improvements
- Share your customizations

-----

**Created with ❤️ for sharing memories with friends**
