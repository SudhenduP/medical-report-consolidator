# Medical Report Tracker

A secure web application for managing and analyzing medical reports with OCR text extraction capabilities.

## Features

- 🔐 **User Authentication** - Secure login/registration system
- 📊 **Patient Dashboard** - Personal health data overview
- 📸 **OCR Processing** - Extract data from uploaded medical reports and photos
- 🎨 **Color-Coded Status** - Visual indicators for test results (Normal, High, Low, Critical)
- 🔍 **Smart Search** - Find reports by test name, date, doctor, or lab
- 📥 **Download Reports** - Export individual reports
- 💾 **Data Persistence** - Reports saved per user account

## Technology Stack

- **Frontend**: React 18, Tailwind CSS
- **Icons**: Lucide React
- **OCR**: Tesseract.js
- **Storage**: LocalStorage (client-side)
- **Deployment**: Vercel

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone 
   cd medical-report-consolidator
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

### Building for Production

```bash
npm run build
```

### Deployment

Deploy to Vercel:
```bash
npm install -g vercel
vercel --prod
```

## Usage

1. **Register/Login** - Create an account or login with existing credentials
2. **Upload Reports** - Click "Upload Report" or "Take Photo" to add medical reports
3. **View Data** - All extracted information appears in the organized table
4. **Search** - Use the search box to find specific tests or dates
5. **Download** - Click the download button to save individual reports

## Supported File Types

- PDF documents
- Images (JPG, JPEG, PNG)
- Camera captures

## OCR Processing

The application uses Tesseract.js for optical character recognition to extract:
- Test names and values
- Reference ranges
- Doctor names
- Lab information
- Test dates

## Color Status Legend

- 🟢 **Normal** - Values within reference range
- 🔴 **High** - Values above reference range
- 🟡 **Low** - Values below reference range
- 🔴 **Critical** - Values requiring immediate attention (pulsing indicator)

## Security & Privacy

- All data stored locally in browser
- No server-side data transmission
- User-specific data separation
- Secure authentication flow

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Tesseract.js for OCR capabilities
- Lucide React for beautiful icons
- Tailwind CSS for styling
- React team for the framework

## Support

For support, email your-email@example.com or open an issue on GitHub.

---

**Note**: This application is for educational purposes. For production use with real medical data, ensure compliance with healthcare regulations (HIPAA, GDPR, etc.).
