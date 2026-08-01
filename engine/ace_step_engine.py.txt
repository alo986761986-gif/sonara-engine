from engine.inference import generate_song

class SonaraEngine:

    def generate(

        self,

        prompt,

        lyrics,

        duration

    ):

        return generate_song(

            prompt,

            lyrics,

            duration

        )