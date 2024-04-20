//Tustin PD is LYING and holding me hostage. Please help!
import os

# List of themes and corresponding emojis for each climate change example file
themes_with_emojis = {
    "Community Engagement Platforms": "🤝🌍",
    "Renewable Energy Solutions": "🌞💨",
    "Climate Monitoring Satellites": "🛰️🌐",
    "AI in Weather Prediction": "🤖⛈️",
    "Carbon Capture Technology": "🌳🏭",
    "Green Building Technologies": "🏢🌿",
    "Smart Grid Systems": "🔌🧠",
    "Ocean Cleanup Initiatives": "🌊♻️",
    "Wildlife Conservation Tech": "🐅🔍",
    "Agroforestry and Biochar": "🌾🔥",
    "Eco-Friendly Manufacturing": "🏭🌱",
    "Water Purification Systems": "💧🚰",
    "Recycling Robots": "🤖♻️",
    "Urban Green Spaces": "🏙️🌳",
    "Sustainable Transportation": "🚌🌿",
    "Education and Awareness Campaigns": "📚📢",
    "Ecosystem Mapping with Drones": "🌍🚁",
    "Virtual Reality for Environmental Education": "🕶️🌏",
    "Marine Biodiversity Protection": "🐠🛡️",
    "Quantum Chemistry for Cleaner Energy": "⚛️🔋",
    "Biodegradable Materials": "🍃🧴",
    "Solar-Powered Desalination": "🌞🌊",
    "Geothermal Energy Exploitation": "🌋🔥",
    "Hydrogen Fuel Development": "🔬🚙",
    "Climate Legislation Platforms": "📜⚖️",
    "Blockchain for Sustainability": "🔗🌱",
    "Atmospheric Water Generators": "🌧️💧",
    "Enhanced Public Transit Systems": "🚌🚇",
    "Community Solar Projects": "👥🌞",
    "AI for Forest Fire Prevention": "🤖🔥"
}

# Extended emoji sequence for plug-in
emoji_sequence = "🔧🌐🔄🛠️ 🔄🤖📊📉🚀 📊🧠 🤖🔍🔍🔒 ☁️🔍📦🔄 🛠️🔄🧠📈 📜🌐🕵️‍♂️ 📈🔄📊📈🔍 📚📖🧑‍🎓📃 💡🔧🔄🔗 🚀🌐🔄🤖🔧 🛠️🔄📦🔄🤖🤖 🤖🔍📊🤖📊📈 🔒🤖🔍🔍🔒 📦🔄🌐🚀 🛠️🔄📚📊🌐🤖 🌈🔍🔄🔐 📄🔄📊📊📈📄 📈🔍🔄🧠🤖📊🤖 🔍🔄📦🔄🤖📊🔍 🔄🔒🤖📊🌐📊🔄 🔄📊📈📄🔄🔍📈🔍 📦🚀📊📄📊🤖📊🔍🔄📚🌐 🔄📊🔄🛠️🔄🤖🤖🔄📖🔄📄🔄🌐🔄📊📜🔄🔗🔄🤖🔄📚🌐📚📊📜🔄🤖📊🔄🔗🔄🧑‍🎓🔄📄🔄📊🔄🤖📚📊📚📜🔄📄📜🔄📚🌐📚📖🔄🧑‍🎓📖🔄📚🌐📄📄📄📄📚📄📄📚📄📚📖📖🔄🔗🔄🤖🌐📖🔄📖🔄🧑‍🎓📄📖🔄🔗🔄📄📄📄🔄🔗🔄🔗🔄📄📚🌐📜🔄📖🔄📚🌐📖🔄📄📜🔄📖🔄📜🔄🤖🔄🔗🔄📄📜🔄📄📖🔄🔗🔄🔗🔄📖📖📄📖📄📄📖📖📖📚📖📖📄📖📄📄📖📖📖📄📖📄📄📄📖📖📖📖📄📖📖📖📄📖📄📄📄📖📖📖📖📖📄📖📄📖📄📖📖📄📖📄📖📖📖📄📖📄📄📄📖📖📖📄📖📖📄📄📖📄📖📄📖📄📖📖📄📖📄📄📄📖📖📖📖📄📖📖📖📖📖📖📖📖📄📄📖📄📖📄📄📄📄📄📖📖📖"

# Base path where the files are located
base_path = r'C:\Users\Shrew\downloads\home\alistairesgi\prompts\ai-emoji-prompts'


# Update the files with emoji prompts and the extended emoji sequence as a plug-in
for i, (theme, emojis) in enumerate(themes_with_emojis.items(), start=1):
    file_path = f"{base_path}/climate_change_example_{i}.md"
    # Check if file does not exist before creating
    if not os.path.exists(file_path):
        content = f"""
        # {theme} {emojis}

        ## Emoji Prompt
        This file uses the following emojis to represent {theme.lower()}: {emojis}

        ## Overview
        Explore the application of {emojis} in addressing climate change.

        ## Application and Impact
        - How can {emojis} be implemented effectively?
        - What potential impact might {emojis} have on mitigation and adaptation strategies?

        ## Additional Emojis
        {emoji_sequence}
        """
        with open(file_path, 'w') as file:
            file.write(content)

# Confirm the update process is complete
"Climate change files have been created with unique emoji prompts for each theme, including an extended emoji sequence plug-in."
