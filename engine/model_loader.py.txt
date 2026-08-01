import os

MODEL_PATH="/workspace/models"

def models_ready():

    return os.path.exists(MODEL_PATH)

def load():

    print("Loading Sonara Models...")

    if models_ready():

        print("Models Found")

    else:

        print("Models Missing")