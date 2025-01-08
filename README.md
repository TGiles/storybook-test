# Minimum Reproducible Storybook

## Dependencies
- Windows 10 or Windows 11
- Enable High Contrast Mode (HCM)

## Issues
- When using the search bar in HCM, matching characters use the background color, effectively becoming invisible. [Screenshot that shows missing characters](./matching_characters_missing.png).
- Some interactive elements do not have hover or focus states, specifically links. When hovering over internal links, say stories or docs within a component, there are no additional indicators that the element is interactive. Having the `cursor: pointer` is helpful, but having some form of underline on links is extremely beneficial in HCM. There are a few ways to handle this:
  - Make underlines appear on hover and focus. This strategy is what [Wikipedia uses for their links](./links_underline_on_hover_wikipedia.png).
  - Always show underlines but make them disappear on hover and focus. MDN uses this for links in the [main content of articles](./links_underline_disappears_on_hover_mdn.png).
  - Always show underlines regardless of hover and focus. This is the default user agent styling in Firefox, seen in this [demo on MDN](./links_underline_always_present_mdn.png)
