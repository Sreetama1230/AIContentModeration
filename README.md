

## Content Moderation

The AI Content Moderation Service analyzes blog posts before they are published to help prevent harmful or inappropriate content from entering the platform.


                REST API
+------------------------------+
|      BlogPost Service        |
+------------------------------+
              |
              | HTTP
              v
+------------------------------+
| Content Moderation Service   |
+------------------------------+
              |
              | HTTPS
              v
      Google Gemini API
      
### How it Works

1. The BlogPost service sends the blog title, content, and categories to the AI Content Moderation Service.
2. The moderation service uses the **Google Gemini API** to evaluate the content against predefined safety guidelines.
3. Based on the AI response, the service either:

   * **Approves** the content for publishing, or
   * **Rejects** the content if it contains harmful, violent, abusive, or illegal material.

### Technologies Used

* Java 17
* Spring Boot
* Google Gemini API
* REST APIs

BlogPostService GitHub Link - https://github.com/Sreetama1230/blogpost_application
