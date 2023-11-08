import json
import yaml
 
# Load JSON file
json_filename = "example.json"
with open(json_filename, "r") as json_file:
    json_data = json.load(json_file)
 
# Load YAML file
yaml_filename = "example.yaml"
with open(yaml_filename, "r") as yaml_file:
    yaml_data = yaml.safe_load(yaml_file)
 
# Extract keys from JSON and YAML
json_keys = set(json_data.keys())
yaml_keys = set(yaml_data.keys())
 
# Compare keys
json_unique_keys = json_keys - yaml_keys
yaml_unique_keys = yaml_keys - json_keys
common_keys = json_keys & yaml_keys
 
# Print the results
print("Keys unique to JSON:", json_unique_keys)
print("Keys unique to YAML:", yaml_unique_keys)
print("Common keys:", common_keys)
