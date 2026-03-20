# ImageHub

A JavaFX-based photo album management application.

## Features
- Login as a user or admin
- Create and manage albums
- Add, delete, move, and copy photos
- Edit photo descriptions and tags
- Search photos by tags
- View photos in a detailed slideshow

---

## Setup Instructions
Before you begin, ensure:
- Java Development Kit (JDK) 21 or higher is installed
- JavaFX SDK 21 is downloaded and extracted

**Important:**  
Replace `/path/to/javafx-sdk-21.0.6/lib` with your actual JavaFX SDK lib path.

---

## Terminal Commands

```bash
# 1. Clean previous builds
rm -rf out

# 2. Create output directory
mkdir -p out

# 3. Compile Java files
javac --module-path /path/to/javafx-sdk-21.0.6/lib --add-modules javafx.controls,javafx.fxml -d out -sourcepath src src/view/*.java

# 4. Copy FXML files
mkdir -p out/view
cp src/view/*.fxml out/view/

# 5. Run the application
java --module-path /path/to/javafx-sdk-21.0.6/lib --add-modules javafx.controls,javafx.fxml -cp out view.Photos



Project Structure：
Photos31/
├── data/
│   ├── users.dat
│   ├── stock_albums.dat
│   └── stock/
│       ├── stock1.jpg
│       ├── stock2.jpg
│       ├── stock3.jpg
│       ├── stock4.jpg
│       └── stock5.jpg
├── docs/
│   └── (Generated Javadoc HTML files)
├── out/
│   └── view/
├── src/
│   └── view/
│       ├── *.java
│       ├── *.fxml
├── .gitignore
├── README.md
├── LICENSE


📜 Notes:
data/ folder contains user data and stock photos.
docs/ folder contains generated Javadoc (open docs/index.html to browse documentation).
Admin can create and delete user accounts.
Regular users can create albums, add photos, and manage tags.
"Stock" user comes preloaded with 5 sample photos in the stock album.


🖥️ Requirements:
Java JDK: 21 or higher
JavaFX SDK: Version 21.0.6
Operating System: macOS, Windows, or Linux







# Author: Alex Yang
