<a id="top"></a>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0F172A,50:4C1D95,200:C026D3&height=200&section=header&text=NEXORA%20AI&fontSize=100&fontColor=ffffff&animation=twinkling&fontAlignY=44&desc=AI-Powered%20Relationship%20Intelligence&descAlignY=70&descSize=20&descColor=e0e7ff" width="100%" alt="Nexora AI — Customer Churn Intelligence"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=25&duration=3000&pause=1000&color=C4B5FD&center=true&vCenter=true&width=660&lines=See+the+goodbye+before+it+happens;Predict+who+will+leave+before+they+do;Explain+every+prediction+with+SHAP;Turn+churn+into+actionable+insight" alt="Tagline"/>

<br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0F172A,50:4C1D95,100:C026D3&height=3" width="60%" alt=""/> 
<br><br>
<img src="https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&labelColor=0F172A&logo=python&logoColor=white" alt="Python 3.10"/>
<img src="https://img.shields.io/badge/Scikit--learn-1.4-F7931E?style=for-the-badge&labelColor=0F172A&logo=scikitlearn&logoColor=white" alt="Scikit-learn 1.4"/>
<img src="https://img.shields.io/badge/FastAPI-0.110-009688?style=for-the-badge&labelColor=0F172A&logo=fastapi&logoColor=white" alt="FastAPI 0.110"/>
<img src="https://img.shields.io/badge/Docker-25-2496ED?style=for-the-badge&labelColor=0F172A&logo=docker&logoColor=white" alt="Docker 25"/>
<img src="https://img.shields.io/badge/Git-2.43-F05032?style=for-the-badge&labelColor=0F172A&logo=git&logoColor=white" alt="Git 2.43"/>
<br><br>
</div>

## Project Layout
 
```text
churniq_website/
├── main.py
├── model.pkl        # Add your trained model file here
├── requirements.txt
└── static/
    ├── index.html
    ├── styles.css
    └── app.js
```

## Run locally

1. Put your existing trained `model.pkl` in the same folder as `main.py`.
2. Open a terminal in this folder.
3. Create and activate a virtual environment (recommended).
4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Start the server:

   ```bash
   uvicorn main:app --reload
   ```

6. Open http://127.0.0.1:8000

The site and API are served from the same FastAPI app, so the frontend can call `/predict` without separate CORS setup. API docs are at http://127.0.0.1:8000/docs.

<!-- <h2>
  <img src="https://cdn.simpleicons.org/docker/74b9ff" width="22" align="absmiddle"/>&nbsp; Docker
</h2> -->

## Important model checks

- This UI assumes the model output `1` means churn and `0` means no churn. Confirm this matches the label encoding used when you trained your model.
- The website intentionally shows the predicted class only. Your API returns no probability, so the UI does not invent a risk percentage.
- The input values must match the categories and feature preprocessing expected by the trained model. In particular, your code maps tenure months into ranges such as `1-12`, `13-24`, etc.
- `paymentmethod`, `internetservice`, `onlinesecurity`, and `techsupport` choices exactly match your current API schema. If the model was trained with different categories (for example, actual payment-method names), update the schema and form options to match training.
- Only run `joblib.load` on a trusted model file.

## API response

The frontend expects `POST /predict` to return JSON like:

```json
{"prediction": 1}
```

</div>
<div align="center">
  
# ✦ NEXORA AI

<div align="center">

<a href="mailto:piyushagarwal146@gmail.com"><img src="https://cdn.simpleicons.org/gmail/ff7675" width="18"/>&nbsp; <b>Mail</b></a>&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://dashefy.vercel.app/"><img src="https://cdn.simpleicons.org/googlechrome/ffeaa7" width="18"/>&nbsp; <b>Portfolio</b></a>&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://www.linkedin.com/in/piyush-agarwal-1a93003a1"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" width="18"/>&nbsp; <b>LinkedIn</b></a>&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://hub.docker.com/repository/docker/piyushagarwal04/nexora_ai/general"><img src="https://cdn.simpleicons.org/docker/74b9ff" width="18"/>&nbsp; <b>Docker</b></a>&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://github.com/YOUR_USERNAME"><img src="https://cdn.simpleicons.org/git/fab1a0" width="18"/>&nbsp; <b>Git</b></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

</div>

<br/>
</div>



