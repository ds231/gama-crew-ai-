# AI Trip Planner 🌍

An intelligent trip planning assistant that uses AI to generate personalized travel itineraries. The application supports multiple AI providers (Google Gemini and Azure OpenAI) and provides detailed trip plans including activities, costs, transportation tips, accommodations, and food recommendations.

## Features ✨

- Multi-AI provider support (Google Gemini and Azure OpenAI)
- Detailed day-by-day trip itineraries
- Budget-aware recommendations
- Location validation
- Transportation and accommodation suggestions
- Local food recommendations
- Cost estimates for activities
- Error handling and input validation
- Free tier friendly (especially with Google Gemini)

## Prerequisites 📋

- Python 3.6+
- Google Colab or Jupyter Notebook
- API key from either:
  - Google Gemini (Recommended for free tier)
  - Microsoft Azure OpenAI (If you have access)

## Installation 🛠️

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-trip-planner.git
cd ai-trip-planner
```

2. Install required packages:
```bash
pip install google-generativeai azure-openai geopy python-dotenv
```

## API Setup 🔑

### Google Gemini (Recommended)
1. Visit [Google MakerSuite](https://makersuite.google.com/app/apikey)
2. Create a free account
3. Generate an API key

### Azure OpenAI (Alternative)
1. You need:
   - Azure OpenAI API key
   - Azure endpoint URL
   - Deployment name
2. Get these from your Azure OpenAI service dashboard

## Usage 💻

1. Run the program:
```bash
python trip_planner.py
```

2. Choose your AI provider:
```
Available AI Providers:
1. Google Gemini (Recommended for free tier)
2. Microsoft Azure OpenAI
```

3. Enter your API credentials when prompted

4. Follow the prompts to enter your trip details:
   - Origin location
   - Destination
   - Start date (YYYY-MM-DD)
   - Duration (1-14 days)
   - Budget (in USD)

## Example Output 📝

```
🌍 Your Trip Plan:
------------------
3-Day Trip to London from India
Budget: $3000

Day 1:
- Morning: Arrive at Heathrow Airport
- Transportation: Heathrow Express to central London ($30)
- Accommodation: Check-in at mid-range hotel in Westminster ($200/night)
...
[Full itinerary details]
```

## Rate Limits 📊

### Google Gemini
- 60 requests per minute (Free tier)
- Perfect for regular use

### Azure OpenAI
- Varies based on your subscription tier
- Check your Azure dashboard for limits

## Error Handling 🔧

The application handles:
- Invalid locations
- API errors
- Rate limiting
- Invalid input formats
- Network issues

## Contributing 🤝

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments 🙏

- Google Gemini API
- Microsoft Azure OpenAI
- Geopy for location validation
- All contributors and users

## Support 💬

For support:
- Open an issue on GitHub
- Contact the maintainers
- Check the documentation

## FAQ ❓

**Q: Which AI provider should I use?**
A: Google Gemini is recommended for free tier users due to its generous limits.

**Q: Is my API key secure?**
A: Your API key is never stored and is only used during runtime.

**Q: Can I use this for commercial purposes?**
A: Yes, but please check the terms of service of your chosen AI provider.

## Troubleshooting 🔍

Common issues and solutions:

1. **API Key Issues**
   - Verify key is correct
   - Check API provider dashboard
   - Ensure you have sufficient credits

2. **Location Validation Fails**
   - Check spelling
   - Use official city names
   - Ensure internet connection

3. **Rate Limiting**
   - Switch to Gemini for higher limits
   - Implement delays between requests
   - Check your usage quotas

## Future Improvements 🚀

- [ ] Add support for more AI providers
- [ ] Implement caching for frequent destinations
- [ ] Add map visualization
- [ ] Include weather forecasts
- [ ] Add multi-language support
- [ ] Create web interface
