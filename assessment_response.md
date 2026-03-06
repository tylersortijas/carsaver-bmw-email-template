# Layout Decisions, CTA Strategy & Compatibility Considerations

## Layout & CTA Strategy

I kept the structure straightforward and familiar so it would hold up well across inboxes. The overall design was heavily inspired by industry standards, and the table-based layout capped at 600px, with a mobile breakpoint at 620px so sections stack cleanly on smaller screens. I also tried to make the content flow feel natural for the reader. It starts with branding to build trust, moves into a clear value proposition in the hero, then walks through the three-step process (Pick It, Price It, Drive It) so the journey feels simple and low-friction. The three CTAs (CHECK YOUR VALUE, EXPLORE BMW MODELS, and START YOUR DEAL) are placed to match different levels of buying intent, but they all point toward the same conversion goal.

Visually, I kept the button treatment consistent in CarSaver blue (#004c91) so the actions are easy to spot and the message feels cohesive from top to bottom.

## Compatibility Considerations

For compatibility, I built in the usual safeguards that email clients still require. Outlook gets VML `v:roundrect` fallbacks through MSO conditional comments, so buttons render correctly even where CSS support is limited. I also added Gmail and Apple Mail data-detector overrides to stop clients from auto-linking random text like dates or phone numbers and breaking styling.

Everything critical is inlined so the email still renders correctly in clients that strip embedded styles, and the template remains readable even with images turned off thanks to alt text and solid background styling. Finally, every link includes UTM parameters so performance can be tracked accurately no matter which CTA the user clicks.
