# Writing Goood Documentation 

## Step 1 - Using codeblocks

**CLoud Engineer**
Codebkocks in markdown make *very easy* for tech people to share code
It allows others to copy and paste thier code to replicate or research issues


Write a code to **Generate an image** with future technologies using python to make it as background image for LinkedIN.


```
from PIL import Image, ImageDraw, ImageFont

# Define image dimensions and background color
width, height = 1584, 396  # LinkedIn background image dimensions
background_color = (51, 102, 153)  # LinkedIn's default blue background color

# Create a new image with the specified dimensions and background color
background = Image.new('RGB', (width, height), background_color)

# Create a drawing object to add text or shapes to the image
draw = ImageDraw.Draw(background)

# Add futuristic elements or text to the image
font_size = 60
font_color = (255, 255, 255)  # White color for text

# You can customize the text and position based on your preference
text = "Srivardhan Tumanapally - Future Technology Enthusiast"
font = ImageFont.truetype("arial.ttf", font_size)
text_width, text_height = draw.textsize(text, font)
text_x = (width - text_width) / 2
text_y = (height - text_height) / 2

draw.text((text_x, text_y), text, font=font, fill=font_color)

# Save the image to a file
background.save("linkedin_background.png")

# Display the image (optional)
background.show()

```

With Syntax Highlighter

```python
from PIL import Image, ImageDraw, ImageFont

# Define image dimensions and background color
width, height = 1584, 396  # LinkedIn background image dimensions
background_color = (51, 102, 153)  # LinkedIn's default blue background color

# Create a new image with the specified dimensions and background color
background = Image.new('RGB', (width, height), background_color)

# Create a drawing object to add text or shapes to the image
draw = ImageDraw.Draw(background)

# Add futuristic elements or text to the image
font_size = 60
font_color = (255, 255, 255)  # White color for text

# You can customize the text and position based on your preference
text = "Srivardhan Tumanapally - Future Technology Enthusiast"
font = ImageFont.truetype("arial.ttf", font_size)
text_width, text_height = draw.textsize(text, font)
text_x = (width - text_width) / 2
text_y = (height - text_height) / 2

draw.text((text_x, text_y), text, font=font, fill=font_color)

# Save the image to a file
background.save("linkedin_background.png")

# Display the image (optional)
background.show()

```

![image](https://github.com/Srivardhan-T/github-docs-example/assets/56570571/e130c13f-e3c7-4484-9444-f6790332c594)

### Use emojis
☁️
🌩️
👍

## References
- [GitHub Flavoured Markdown Spec](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

