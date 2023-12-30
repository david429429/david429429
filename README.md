- 👋 Hi, I’m @david429429
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
david429429/david429429 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
ENDPOINT = https://api-inference.huggingface.co/modelsfrom gradio_client import Client

client = Client("https://prt429-outfitanyone.hf.space/--replicas/otqex/")
result = client.predict(
		0,	# int (index of selected example) in 'parameter_5' Dataset component
							api_name="/load_example"
)
print(result)
