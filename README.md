Thumbnail Generator
Overview
A web-based image processing application that allows users to upload images, automatically generate thumbnails, and manage files through MinIO object storage and MongoDB database integration.​

Live URL: https://image-pipeline-project-six.vercel.app/

Features & Functionality
1. 🏠 Dashboard
The main landing page provides an overview of the application and quick access to key features.​

Key Features:

Image Upload Zone: Drag-and-drop interface or click-to-browse functionality

File Support: JPG and PNG formats supported

Upload Behavior: Uploads original size without cropping by default

Processed Assets Display: Shows previously uploaded and processed images from the server

Quick Access: Summary of application capabilities - "Upload images. Auto-generate thumbnails. Store and process files via MinIO."

2. ⬆️ Upload & Crop
Dedicated page for uploading images with advanced cropping and resizing options.​

Key Features:

File Selection: Standard file upload interface ("Choose File" button)

Size Presets: Dropdown menu with multiple size options:

Original Size (default)

Thumbnail (200x200)

Small (640x480)

Medium (1280x720)

Purpose: Select source image to crop and apply initial resizing before processing

3. 🗄️ MinIO Browser
Interface for browsing and managing files stored in MinIO object storage.​

Key Features:

Bucket Browsing: Displays contents of MinIO bucket via API integration

External Console Access: Direct link to dedicated MinIO console (http://localhost:9001)

Purpose: View and manage stored image files in the object storage system

4. 📝 MongoDB Items
Database viewer for tracking image metadata and processing status.​

Key Features:

Database Connection Status: Shows connection status to BytexlDB ("Connected to BytexlDB")

Records Display: Displays detailed table of all records including:

Metadata information

Processing status

Collection: Data stored in MongoDB collection called "imagerecords"

5. ⚙️ Settings
Application configuration and preferences management.​

Key Features:

Theme Management:

Current theme display (Light/Dark)

Toggle button: "Switch to Dark Mode 🌙"

Global theme management across all pages

Application Preferences: Centralized settings control

Note: Theme toggling is globally managed by the Dashboard Layout

User Interface
Navigation
Sidebar Menu: Persistent left sidebar with navigation links to all sections

Theme Toggle: Moon icon (🌙) in top-right corner for quick theme switching

Active Page Indicator: Highlighted menu item shows current page

Logo: Thumbnail Generator branding with image icon at top of sidebar

Design Elements
Clean, modern interface with blue accent colors

Responsive layout with sidebar navigation

Card-based content sections

Light/Dark mode support

Icon-based navigation for better UX

Technical Stack
Backend Services
MinIO: Object storage for image files

MongoDB: Database for metadata and processing records (BytexlDB)

API Integration: Server-side processing for thumbnail generation

Storage Architecture
Original images stored in MinIO buckets

Metadata tracked in MongoDB "imagerecords" collection

Automated thumbnail generation pipeline

Supported Operations
Upload images (JPG, PNG formats)

Auto-generate thumbnails in multiple sizes

Crop and resize images before processing

Browse stored files in MinIO

View processing metadata in MongoDB

Manage application settings and themes

File Processing Pipeline
User uploads image via Dashboard or Upload & Crop page

Optional: Apply cropping and size preset

Original file stored in MinIO bucket

Thumbnail variants auto-generated

Metadata saved to MongoDB

Processed assets displayed on Dashboard

