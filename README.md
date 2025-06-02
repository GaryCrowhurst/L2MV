# 📱 Level 2 Light Vehicle Photo Evidence Tracker

A mobile-first web application designed for automotive learners to track their progress through Level 2 Light Vehicle Maintenance & Repair qualifications by uploading photographic evidence for each required task.

## 🎯 Purpose

This application helps automotive students and apprentices:
- **Track Progress** through 35 required evidence tasks across 4 core units
- **Upload Photos** directly from mobile cameras or device galleries
- **Generate Professional PDFs** for portfolio submission
- **Maintain Evidence** offline with local storage backup
- **Cross-Reference Tasks** with clear unit relationships

## 📚 Curriculum Coverage

### Core Units Tracked:
- **4290-001** - Health, Safety & Good Housekeeping (3 tasks)
- **4290-004** - Materials, Fabrication, Tools & Measuring (3 tasks)  
- **4290-101** - Routine Light Vehicle Maintenance (5 tasks)
- **4290-104** - Chassis Units & Components (24 tasks)
  - 🚗 Brake System (A1-A10)
  - 🔧 Suspension System (B1-B7) 
  - 🎯 Steering System (C1-C6)

## ✨ Key Features

### 📸 **Smart Photo Upload**
- **Dual Upload Options**: Camera capture or gallery selection
- **Mobile Action Sheet**: Touch-friendly photo source selection
- **Auto-Compression**: Optimizes images for mobile performance
- **Drag & Drop Support**: Desktop file handling

### 📊 **Progress Tracking**
- **Visual Progress Bars**: Overall and section-specific completion
- **Task Dependencies**: Cross-references between related tasks
- **Completion Validation**: Photos required before task marking
- **Real-time Updates**: Instant progress calculation

### 🔍 **Advanced Search & Filter**
- **Live Search**: Find tasks by name, description, or unit code
- **Filter Options**: All tasks, completed, or pending
- **Auto-expand**: Search results automatically expand relevant sections
- **Highlight Terms**: Visual emphasis on search matches

### 📄 **Professional PDF Generation**
- **Complete Portfolios**: All evidence in submission-ready format
- **Partial Export**: Generate PDFs with current progress
- **Structured Layout**: Organized by unit and system sections
- **Metadata Included**: Learner name, completion status, generation date

### 💾 **Data Management**
- **Auto-save**: Continuous local storage backup
- **Export/Import**: JSON backup files for data portability
- **Offline Capability**: Full functionality without internet
- **Cross-device Sync**: Manual backup/restore workflow

## 🚀 Quick Start

### Option 1: Direct Use
1. **Download** the HTML file to your device
2. **Open** with any modern web browser
3. **Add to Home Screen** on mobile for app-like experience
4. **Start uploading** evidence photos

### Option 2: Web Server
```bash
# Simple HTTP server (Python)
python -m http.server 8000

# Or with Node.js
npx http-server

# Navigate to http://localhost:8000
```

### Option 3: GitHub Pages
1. Fork this repository
2. Enable GitHub Pages in repository settings
3. Access via: `https://yourusername.github.io/repo-name`

## 📱 Mobile Installation

### iOS (Safari)
1. Open the app in Safari
2. Tap the **Share** button
3. Select **"Add to Home Screen"**
4. Enjoy full-screen app experience

### Android (Chrome)
1. Open the app in Chrome
2. Tap the **Menu** (three dots)
3. Select **"Add to Home screen"**
4. Confirm installation

## 🎮 Usage Guide

### Getting Started
1. **Enter Your Name**: Required for PDF portfolio generation
2. **Expand Units**: Tap unit headers to view tasks
3. **Upload Evidence**: Use camera or select from gallery
4. **Mark Complete**: Check tasks after photo upload
5. **Track Progress**: Monitor completion in progress section

### Best Practices
- 📸 **Take Clear Photos**: Ensure work and tools are visible
- 💾 **Export Regularly**: Backup progress to prevent data loss
- 🏷️ **Name Photos Clearly**: Original filenames are preserved
- ✅ **Complete Sequentially**: Follow logical task progression
- 📱 **Use Mobile**: Optimized for on-site photo capture

### PDF Portfolio Generation
1. **Click "Download Evidence PDF"**
2. **Choose Complete or Partial** export
3. **Save File** to device or cloud storage
4. **Submit** to assessor or upload to learning platform

## 🛠️ Technical Specifications

### Dependencies
- **Tailwind CSS**: Responsive styling framework
- **Lucide Icons**: Lightweight icon library
- **jsPDF**: Client-side PDF generation
- **Browser APIs**: File, Camera, LocalStorage

### Browser Compatibility
- ✅ **Chrome/Edge**: Full feature support
- ✅ **Safari**: Full iOS/macOS compatibility
- ✅ **Firefox**: Complete functionality
- ✅ **Mobile Browsers**: Optimized experience

### Performance Features
- **Image Compression**: 1200px max dimension, 80% JPEG quality
- **Lazy Loading**: Progressive task rendering
- **Local Storage**: Efficient state management
- **Touch Optimization**: 44px minimum touch targets

### Security & Privacy
- **No Server Required**: Fully client-side operation
- **Local Data Storage**: Photos never leave your device
- **No Analytics**: Complete privacy protection
- **Offline First**: No internet dependency

## 📂 File Structure

```
evidence-tracker/
├── index.html              # Main application file
├── README.md               # This documentation
├── assets/                 # Static assets (if using)
│   ├── icons/             # PWA icons
│   └── screenshots/       # Documentation images
└── docs/                  # Additional documentation
    ├── user-guide.md      # Detailed user instructions
    └── technical-guide.md # Developer documentation
```

## 🔧 Customization

### Adding New Tasks
```javascript
// In UNITS_DATA array, add new task object:
{
    id: 'NEW-TASK-ID',
    label: 'Task Name',
    description: 'Detailed task description',
    uploadLabel: 'Upload Photo – Description',
    crossRef: 'Optional cross-reference info'
}
```

### Styling Modifications
- **CSS Variables**: Modify color scheme in `:root`
- **Responsive Breakpoints**: Adjust mobile-first media queries
- **Component Styling**: Target specific CSS classes

### Feature Extensions
- **New Units**: Extend `UNITS_DATA` structure
- **Additional Fields**: Enhance task data model
- **Export Formats**: Add alternative download options

## 🤝 Contributing

### Bug Reports
1. **Check Existing Issues** before creating new ones
2. **Include Browser/Device** information
3. **Provide Steps to Reproduce** the issue
4. **Add Screenshots** if applicable

### Feature Requests
1. **Describe Use Case** and benefits
2. **Consider Mobile Impact** for all suggestions
3. **Maintain Educational Focus** of the application

### Development Guidelines
- **Mobile-First Design**: Always consider mobile experience
- **Accessibility**: Maintain WCAG compliance
- **Performance**: Optimize for slow networks
- **Progressive Enhancement**: Ensure basic functionality works everywhere

## 📞 Support

### Common Issues

**Q: Photos not saving?**
A: Check browser storage limits and try exporting/clearing old data

**Q: PDF generation failing?**
A: Ensure photos are compressed and browser has sufficient memory

**Q: App not working offline?**
A: Check if service worker registered successfully in browser dev tools

**Q: Lost progress?**
A: Import from previously exported JSON backup file

### Educational Support
- **Assessment Guidance**: Consult your course handbook
- **Technical Issues**: Contact your IT support team
- **Portfolio Requirements**: Check with your assessor

## 📜 License

This project is released under the **MIT License**.

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
```

## 🌟 Acknowledgments

- **Automotive Education Community** for curriculum requirements
- **Open Source Contributors** for underlying technologies
- **Beta Testers** from automotive training programs
- **Mobile Web Standards** working groups

## 📈 Roadmap

### Planned Features
- 🔄 **Cloud Sync**: Optional cloud backup integration
- 📊 **Analytics Dashboard**: Progress insights and statistics
- 👥 **Multi-user Support**: Instructor oversight capabilities
- 🏆 **Achievement System**: Gamification elements
- 📝 **Note Taking**: Additional context for each photo
- 🔍 **QR Code Scanning**: Quick task identification

### Version History
- **v2.0** - Mobile action sheet, dual upload options
- **v1.5** - Advanced search and filtering
- **v1.0** - Initial release with core functionality

---

**Built with ❤️ for automotive education**

*Supporting the next generation of automotive technicians with modern digital tools*
