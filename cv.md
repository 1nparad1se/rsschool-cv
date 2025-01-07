# Jeyhun Ismailov

![photo](https://i.imgur.com/329UwUR.png)

## Contact Information
- **Telegram:** [InParad1se](https://t.me/InParad1se)
- **VK:** [1nparad1se](https://vk.com/1nparad1se)

## About Me
I started getting interested in programming about 2-2.5 years ago. I have knowledge of the Python programming language and have written Telegram bots using aiogram. Initially, I did not have the goal of becoming a developer when I started learning Python. Currently, I work as a QA Engineer and frequently interact with developers. Through these interactions, I realized that I am interested in Frontend development. My colleagues recommended this school, which they also attended. I am highly motivated to become a Frontend developer.

## Skills
- **Programming Languages:** Python
- **Frameworks:** Aiogram
- **Tools:** DevTools, Postman, Charles, Git, YouTrack

## Code Examples
```python
async def csgo2_check_updates():
    global csgo2_update
    try:
        response = requests.get(url_csgo2)
        csgo2_json = response.json()
        title = csgo2_json['events'][0]['event_name']
        link = "https://www.counter-strike.net/news/updates"
        image_src = "https://cdn.akamai.steamstatic.com/apps/csgo/images/csgo_react/social/cs2.jpg"
        ik_csgo2 = InlineKeyboardMarkup(row_width=2)
        b_csgo2 = InlineKeyboardButton("Подробнее", url=link)
        ik_csgo2.add(b_csgo2)
        # Проверяем наличие обновления
        if title != csgo2_update:
            csgo2_update = title
            await bot.send_photo(photo=image_src,
                                 parse_mode='HTML',
                                 chat_id=chat_id,
                                 caption=f"CS:GO2 - {csgo2_update}\n"
                                         f"{hlink('Подробнее', link)}")
    except Exception as e:
        print("Ошибка при выполнении запроса CS:GO2:", e)
```

## Work Experience
- **QA Engineer** (11 months)

## Education
- **MGGEU Volgograd** - Applied Informatics

## English Proficiency
- **Level:** A2
