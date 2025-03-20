<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twitter Sentiment Analysis</title>
    <style>
        /* Basic styling for the video box */
        .video-container {
            width: 80%;
            max-width: 800px;
            margin: 20px auto;
            border: 1px solid #ddd;
            padding: 10px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        .video-container h2 {
            margin-bottom: 10px;
        }

        .video-container iframe {
            width: 100%;
            height: 400px; /* Adjust height as needed */
            border: none;
        }

        /* Rest of your existing CSS or link to your stylesheet */
    </style>
</head>
<body>

    <div class="video-container">
        <h2>Application Demo Video</h2>
        <iframe 
            src="https://www.youtube.com/embed/YOUR_YOUTUBE_VIDEO_ID" 
            title="Twitter Sentiment Analysis Demo" 
            frameborder="0" 
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
            allowfullscreen>
        </iframe>
    </div>

    <h1>Twitter Sentiment Analysis</h1>

    <h2>Project Overview</h2>
    <p>This project implements a machine learning-based sentiment analysis system for Twitter reviews. It uses a Logistic Regression model trained on the Sentiment140 dataset to classify text as either positive or negative sentiment.</p>

    <h2>Dataset Information</h2>
    <p>The model is trained on the Sentiment140 dataset which contains:</p>
    <ul>
        <li>1.6 million tweets</li>
        <li>Binary sentiment classification (0 = negative, 1 = positive)</li>
        <li>Features include: target, ids, date, flag, user, and text</li>
    </ul>

    <h2>Technical Stack</h2>
    <ul>
        <li><strong>Frontend</strong>: HTML, CSS, JavaScript</li>
        <li><strong>Backend</strong>: Flask (Python)</li>
        <li><strong>Machine Learning</strong>: Scikit-learn, NLTK</li>
        <li><strong>Database</strong>: SQLite</li>
    </ul>

    <h2>Model Architecture</h2>
    <p>The sentiment analysis model uses:</p>
    <ul>
        <li>Text preprocessing and cleaning</li>
        <li>CountVectorizer for feature extraction</li>
        <li>Logistic Regression classifier</li>
        <li>Achieved accuracy: 78.39%</li>
    </ul>

    <h2>API Usage</h2>
    <p>The sentiment analysis endpoint can be accessed via POST request:</p>
    <pre><code>
POST /predict
Content-Type: application/x-www-form-urlencoded

Body: review=your_text_here
    </code></pre>
    <p>Response format:</p>
    <pre><code>
{
    "prediction": "Positive/Negative",
    "status": "success"
}
    </code></pre>

    <h2>Features</h2>
    <ul>
        <li>Real-time sentiment analysis</li>
        <li>User authentication system</li>
        <li>Responsive design</li>
        <li>Dark mode support</li>
        <li>Contact form functionality</li>
    </ul>

    <h2>Installation</h2>
    <p>To run the project locally:</p>
    <ol>
        <li>Clone the repository</li>
        <li>Install dependencies: <code>pip install -r requirements.txt</code></li>
        <li>Run the Flask application: <code>python app.py</code></li>
        <li>Access at: <code>http://localhost:5000</code></li>
    </ol>

</body>
</html>
