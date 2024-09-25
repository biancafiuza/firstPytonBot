# Verify if the request was successful (code 200)
if response.status_code == 200:
    # Parse content page using BeautifulSoup
    soup = BeautifulSoup(response.text, 'html.parser')
    
    # Finding titles on pages
    titles = soup.find_all('h2')  # Suponse titles are <h2>

    # Show titles in console
    print("Articles Titles:")
    for title in titles:
        print(title.get_text(strip=True))  # Get text and remove extra spaces
else:
    print(f"Error acessing page: {response.status_code}")
