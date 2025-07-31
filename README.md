# Sohaib GYM - Ad Management System

A comprehensive advertising platform that allows end users to create targeted advertisements with specific details based on subcategories. Built with modern HTML, CSS, and JavaScript.

## 🚀 Features

### For End Users

#### 1. **Category-Based Ad Creation**
- **5 Main Categories**: Fitness & Health, Sports & Recreation, Wellness & Spa, Nutrition & Supplements, Equipment & Gear
- **Dynamic Subcategories**: Each category has specific subcategories with tailored form fields
- **Smart Form Fields**: Different input fields appear based on the selected subcategory

#### 2. **Subcategory-Specific Details**
The system automatically shows relevant fields based on the selected subcategory:

**Personal Training:**
- Years of Experience
- Certifications
- Specialties
- Session Length

**Group Classes:**
- Maximum Class Size
- Class Level (Beginner/Intermediate/Advanced/All Levels)
- Class Schedule

**Cardio Training:**
- Equipment Used
- Intensity Level
- Session Duration

**Protein Supplements:**
- Protein Type (Whey/Casein/Plant-based/Blend)
- Serving Size
- Available Flavors

**Cardio Equipment:**
- Equipment Type (Treadmill/Elliptical/Bike/Rower/StairMaster)
- Brand
- Condition (New/Like New/Good/Fair)

#### 3. **Comprehensive Ad Management**
- **Dashboard Overview**: View all ads with statistics
- **Search & Filter**: Find ads by title, category, or status
- **Edit & Delete**: Manage existing advertisements
- **Status Tracking**: Active, Pending, and Expired ad statuses

#### 4. **Media Support**
- Image upload with preview
- Automatic image optimization
- Visual ad preview before submission

## 📁 File Structure

```
├── index.html              # Main navigation page
├── ad-creation.html        # Ad creation form with dynamic fields
├── ad-dashboard.html       # Ad management dashboard
├── LandingPage.html        # Original gym landing page
├── SurveyForm.html         # Contact form
├── Documentation.html      # Documentation page
├── Freecode.html          # Additional content
└── README.md              # This documentation
```

## 🎯 How to Use

### For End Users

#### 1. **Creating an Ad**

1. **Navigate to Ad Creation**
   - Open `index.html` in your browser
   - Click "Create New Ad" or navigate to `ad-creation.html`

2. **Fill Basic Information**
   - Enter ad title and description
   - Select ad type (Promotion/Event/Service/Product)

3. **Choose Category & Subcategory**
   - Select main category (e.g., "Fitness & Health")
   - Choose subcategory (e.g., "Personal Training")
   - **Dynamic fields will automatically appear** based on your selection

4. **Add Specific Details**
   - Fill in the subcategory-specific fields that appear
   - For Personal Training: Add experience, certifications, specialties, session length
   - For Equipment: Specify brand, condition, equipment type

5. **Upload Media**
   - Add images to your ad
   - Preview uploaded images before submission

6. **Contact Information**
   - Provide contact name, phone, and email
   - Set pricing and ad duration

7. **Submit**
   - Preview your ad before final submission
   - Submit for review

#### 2. **Managing Your Ads**

1. **Access Dashboard**
   - Navigate to `ad-dashboard.html`
   - View all your submitted ads

2. **Search & Filter**
   - Use search bar to find specific ads
   - Filter by category or status
   - View statistics (Total, Active, Pending, Expired ads)

3. **Edit Ads**
   - Click "Edit" on any ad card
   - Modify title, description, price, or status
   - Save changes

4. **Delete Ads**
   - Click "Delete" to remove ads
   - Confirm deletion

## 🔧 Technical Implementation

### Dynamic Form Fields

The system uses JavaScript to dynamically show/hide form fields based on subcategory selection:

```javascript
const subcategoryFields = {
    'Personal Training': [
        { name: 'experience', label: 'Years of Experience', type: 'number' },
        { name: 'certifications', label: 'Certifications', type: 'text' },
        // ... more fields
    ],
    // ... other subcategories
};
```

### Category Mapping

Categories and subcategories are mapped for easy management:

```javascript
const categoryMap = {
    'fitness': [
        'Personal Training',
        'Group Classes',
        'Cardio Training',
        // ... more subcategories
    ],
    // ... other categories
};
```

### Form Validation

- Required field validation
- Email format validation
- File type validation for images
- Real-time form validation

## 🎨 Design Features

### Modern UI/UX
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Gradient Backgrounds**: Modern visual appeal
- **Smooth Animations**: Hover effects and transitions
- **Card-Based Layout**: Clean, organized presentation

### User Experience
- **Intuitive Navigation**: Easy-to-use interface
- **Visual Feedback**: Success/error messages
- **Preview Functionality**: See ad before submission
- **Mobile-Friendly**: Optimized for all devices

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server setup required (runs locally)

### Installation
1. Download all HTML files to a folder
2. Open `index.html` in your web browser
3. Start creating and managing ads!

### Local Development
```bash
# If you have Python installed
python -m http.server 8000

# If you have Node.js installed
npx serve .

# Then open http://localhost:8000 in your browser
```

## 📊 Sample Data

The dashboard includes sample ads to demonstrate functionality:

1. **Personal Training Sessions** - Active ad with trainer details
2. **Protein Supplements Sale** - Pending ad with product specifications
3. **Cardio Equipment - Treadmill** - Active ad with equipment details

## 🔮 Future Enhancements

### Planned Features
- **User Authentication**: Login system for ad management
- **Database Integration**: Persistent data storage
- **Advanced Analytics**: Ad performance tracking
- **Payment Integration**: Paid ad placement
- **Admin Panel**: Content moderation tools
- **API Integration**: Third-party service connections

### Technical Improvements
- **Backend Development**: Server-side processing
- **Database Design**: Structured data storage
- **API Development**: RESTful API for mobile apps
- **Security Features**: Data encryption and validation

## 🤝 Contributing

To contribute to this project:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Support

For support or questions:
- Email: support@sohaibgym.com
- Phone: +1234567890
- Website: [Sohaib GYM](https://sohaibgym.com)

---

**Built with ❤️ for the fitness community**