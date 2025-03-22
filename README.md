import json

# Read data from the .txt file
with open("data.txt", "r", encoding="utf-8") as txt_file:
    lines = txt_file.readlines()

# Convert lines into a dictionary
data_dict = {}
for line in lines:
    key_value = line.strip().split(":", 1)  # Split only on the first colon
    if len(key_value) == 2:
        key, value = key_value
        data_dict[key.strip()] = value.strip()

# Write data to a .json file
with open("data.json", "w", encoding="utf-8") as json_file:
    json.dump(data_dict, json_file, indent=4)

print("Conversion completed: 'data.json' created.")
