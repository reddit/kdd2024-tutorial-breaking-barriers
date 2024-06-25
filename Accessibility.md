# Accessibility

Interesting references:
- [The A11Y Project](https://www.a11yproject.com/). a11y stands for ACCESSIBILITY.
- [IBM Accessibility](https://www.ibm.com/able/). Accessibility is a team effort.
- [Microsoft Innovation and AI for Accessibility](https://www.microsoft.com/en-us/accessibility/). Raising the bar on accessibility.

## Web Content Accessibility Guidelines

[Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/) is a set of guidelines published by the World Wide Web Consortium for making web content accessible to people with disabilities, encompassing a wide range of impairments like blindness, deafness, limited movement, and cognitive limitations. While not addressing every individual need, WCAG 2.1 offers testable criteria across various devices, promoting inclusivity and usability for all users. 

Guidelines cover several relevant dimensions:

- Perceivable:

  - **Text Alternatives**: Ensuring all non-text content like images, videos, and audio have text alternatives for screen readers.
  - **Time-based Media**: Providing captions for videos, audio descriptions for visually impaired users, and transcripts for audio content.
  - **Adaptable**: Making sure information is presented in a logical order and can be understood regardless of how it is displayed (e.g., mobile vs. desktop).
  - **Distinguishable**: Sufficient color contrast for text and UI elements to aid users with visual impairments. Also, providing controls for audio that plays automatically.

- Operable:
  - **Keyboard Accessible**: Ensuring all functionality can be accessed and used with a keyboard, as some users cannot use a mouse.
  - **Enough Time**: Providing users with sufficient time to complete tasks, especially if there are time limits involved.
  - **Seizures and Physical Reactions**: Avoiding content that could trigger seizures, such as flashing images.
  - **Navigable**: Clear and consistent navigation mechanisms, headings, and labels.
  - **Input Modalities**: Supporting different input methods (like touch, mouse, and keyboard) and providing alternatives for complex gestures.

- Understandable:
  - **Readable**: Clear and concise language, appropriate reading level.
  - **Predictable**: Consistent layout and behavior of website elements.
  - **Input Assistance**: Helping users avoid and correct mistakes when filling out forms or providing input.

- Robust:
  - **Compatible**: Ensuring compatibility with different browsers and assistive technologies.

In general, all general web accessibility guidelines apply to social media. However, among all guidelines, the ones that would most apply to the use case of social media such as Reddit are:
- [Guideline 1.1 Text Alternatives](https://www.w3.org/TR/WCAG21/#text-alternatives)
- [Guideline 1.2 Time-based Media](https://www.w3.org/TR/WCAG21/#time-based-media)

### Guideline 1.1: Text Alternatives

This section of the WCAG 2.1 guidelines focuses on the principle of Perceivable information. Specifically, it emphasizes the need for text alternatives for all non-text content. This ensures that information conveyed through visuals, audio, or other non-textual formats can be transformed into accessible formats like braille, large print, speech, symbols, or simpler language.

#### Success Criterion 1.1.1: Non-text Content (Level A)

This criterion requires that all non-text content presented to the user has a text alternative that serves the equivalent purpose. This means any information conveyed visually must also be available in text form.

There are several exceptions to this rule:

- **Controls and Input**: Non-text content used as controls or for user input must have a name that describes its purpose.
- **Time-Based Media**: Text alternatives for time-based media (audio and video) need only provide descriptive identification, with further requirements outlined in Guideline 1.2.
- **Tests**: Text alternatives for tests or exercises that would be invalidated if presented in text form should descriptively identify the non-text content.
- **Sensory Experiences**: Primarily sensory content should also have a text alternative that identifies and describes it.
- **CAPTCHA**: CAPTCHA must have text alternatives identifying their purpose and offer alternative forms that accommodate various sensory perceptions.
- **Decoration, Formatting, Invisible**: Purely decorative, formatting-related, or invisible content can be ignored by assistive technologies.

This Success Criterion ensures that users who cannot perceive non-text content, due to disabilities like blindness or visual impairment, can still access the information and functionality of the website.

### Guideline 1.2 Time-based Media

This section focuses on providing alternatives for time-based media, encompassing both pre-recorded and live content. It emphasizes the importance of catering to users who cannot perceive auditory or visual information directly. This includes providing captions, audio descriptions, and alternative media formats to ensure that content is accessible to individuals with various disabilities.

#### Success Criterion 1.2.3: Audio Description or Media Alternative (Prerecorded) (Level A)

This criterion mandates that pre-recorded synchronized media, primarily video content, should have either audio descriptions or a time-based media alternative available. This does not apply if the media is already serving as a text alternative and is clearly labeled as such.

- **Audio Description**: This involves adding narration to the existing soundtrack, describing visual details that are not conveyed through the existing audio. This helps users who are blind or visually impaired understand the visual aspects of the content.

- **Time-based Media Alternative**: This involves providing an alternative format that presents the same information as the video in a text-based or auditory manner. This could be a transcript, a detailed textual description, or a separate audio track that conveys the visual information.

This criterion ensures that users who cannot perceive visual information can still access the essential content of the pre-recorded video.
