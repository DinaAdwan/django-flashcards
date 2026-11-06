# Django Flashcards

A flashcards app built with Django during the Gaza Sky Geeks backend programme, using a Leitner-style box system for spaced repetition.

## Features
- Create, edit and delete flashcards (question and answer)
- Cards live in 5 boxes: answering correctly moves a card up a box, a wrong answer sends it back to box 1
- Box view picks a random card from the box to quiz you
- Custom template tags for the box navigation
- Class-based views (`ListView`, `CreateView`, `UpdateView`, `DeleteView`)

## Tech
Python · Django 4.1 · SQLite · Django templates

## Run locally
```bash
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The secret key is read from the `DJANGO_SECRET_KEY` environment variable; a development fallback is used if it isn't set.
