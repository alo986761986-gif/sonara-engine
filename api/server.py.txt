from fastapi import FastAPI
from api.routes import router

app = FastAPI(
    title="Sonara AI Engine",
    version="1.0.0"
)

app.include_router(router)

@app.get("/")
def home():
    return {
        "engine": "Sonara",
        "status": "online",
        "gpu": "RTX4090"
    }