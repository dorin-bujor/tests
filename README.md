# Java Programming Exam

This exam is designed to help a student practice and learn Java by creating a real-world application involving art. The exam focuses on topics such as abstract classes, interfaces, inheritance, string manipulation, and error handling.

---

## Part 1: Abstract Class and Interface Design

### Question 1: Define an abstract class `ArtPiece`
- **Attributes**:
  - `title` (String)
  - `artistName` (String)
  - `description` (String)
- **Methods**:
  - An abstract method `displayDetails()` that shows the specific details of the artwork.
  - A method `formatDescription(String description)` to:
    - Trim unnecessary spaces.
    - Capitalize the first letter of every sentence.
    - Replace any occurrence of `"painting"` with `"masterpiece"`.

---

### Question 2: Define an interface `Critiqueable`
- **Methods**:
  - `addCritique(String critique)` to add critiques for an art piece.
  - `getCritiqueSummary()` to display all critiques for the art piece.
- **Error Handling**:
  - If a critique is empty, throw an exception: `"Critique cannot be empty."`
  - If a critique exceeds 200 characters:
    - Truncate it.
    - Display a warning: `"Critique truncated to 200 characters."`

---

### Question 3: Create a concrete class `Painting`
- **Inheritance**:
  - Extends `ArtPiece` and implements `Critiqueable`.
- **Attributes**:
  - `medium` (e.g., oil, watercolor).
- **Methods**:
  - Implement `displayDetails()` to include painting-specific details.
  - Implement the methods from the `Critiqueable` interface.

---

### Question 4: Create a concrete class `Sculpture`
- **Inheritance**:
  - Extends `ArtPiece` and implements `Critiqueable`.
- **Attributes**:
  - `material` (e.g., marble, bronze).
- **Methods**:
  - Implement `displayDetails()` to include sculpture-specific details.
  - Implement the methods from the `Critiqueable` interface.

---

## Part 2: Class Relationships and Inheritance

### Question 5: Define a class `Artist`
- **Attributes**:
  - `name` (String)
  - `bio` (String)
  - A collection of `ArtPiece` objects (their works).
- **Methods**:
  - `addArtPiece(ArtPiece artPiece)` to add an artwork to the artist's collection.
  - `getPortfolio()` to display the artist’s bio and their artworks.

---

### Question 6: Create a class `Exhibition`
- **Attributes**:
  - A collection of `ArtPiece` objects.
- **Methods**:
  - `addToExhibition(ArtPiece artPiece)` to add an artwork to the exhibition.
  - `displayExhibitionDetails()` to list all artworks in the exhibition, along with their critiques.

---

## Part 3: Additional Features

### Question 7: Add sorting functionality for artworks
- **Method**:
  - `sortArtPiecesByTitle()` in the `Exhibition` class to sort all artworks alphabetically by their title.

---

### Question 8: Implement a search feature
- **Method**:
  - `searchArtPiece(String keyword)` in the `Exhibition` class to find all artworks where the title or description contains the keyword (case-insensitive).

---

### Question 9: Implement meaningful string manipulation in `Exhibition`
- **Method**:
  - `cleanTitles()` to:
    - Convert all titles to lowercase.
    - Replace any special characters in titles with spaces.
    - Capitalize the first letter of each word in the title.

---

### Question 10: Add error handling for invalid artwork additions
- **Validation**:
  - Ensure an `ArtPiece` cannot be added to an artist or exhibition if:
    - Its title is empty. Throw an exception: `"Title cannot be empty."`
    - The artist’s name is missing. Throw an exception: `"Artist name cannot be empty."`

---

## Part 4: Final Application

### Question 11: Build the full application
- **Demonstrate the following in a `main()` method**:
  1. Create multiple `Artist` objects, each with a portfolio of `Painting` and `Sculpture` objects.
  2. Add these artworks to an `Exhibition`.
  3. Add and retrieve critiques for several artworks.
  4. Format descriptions using the `formatDescription()` method.
  5. Sort and display all artworks in the exhibition.
  6. Search for artworks based on keywords in their title or description.
  7. Use `cleanTitles()` to standardize artwork titles.
  8. Display the details of the exhibition, including all artworks, their critiques, and the artists who created them.

--- 

Good luck with the exam!
