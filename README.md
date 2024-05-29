# GrandMA LLM

## Motivations

"In Africa, when an old man dies, a library burns," said Senegalese writer Amadou Hampâté-Bâ. This quote perfectly illustrates the importance of elders in preserving the cultural heritage of the continent and passing down knowledge. Given the fleeting nature of life, it is crucial for each of us to consider ways to preserve these heritage elements that are part of our DNA.

Today, with the development of AI and the emergence of LLMs, it is possible to contribute to this endeavor. The goal of our project is precisely in this direction. We aim to leverage the power of such technologies to preserve African culture through tales.

More specifically, our solution, "GrandMA LLM," is based on a collection of tales extracted from various sources and different African countries, reflecting each country's folklore. The goal is to draw inspiration from these tales to generate custom-made original stories that respect African traditions and customs.

Given the scarcity of solutions that include African languages and the need to democratize AI in our continent, we wanted to make this solution multilingual to facilitate its use by people who do not necessarily understand foreign languages. To this end, prompts can be written in Wolof, Moroccan Arabic, Swahili, Bambara, etc., and receive text in these languages in return.

## Architecture

Our architecture is structured as follows:
1. **Scraping and monitoring tales** from multiple sources (PDF, HTML, raw data, etc.) and various countries (Mali, Morocco, Algeria, etc.).
2. **Processing and structuring this data** (grouping by tale, country, language, etc.).
3. **Translating non-English data into English**.
4. **Implementing a RAG architecture using Falcon**.
5. **Fire!** (Conversation with GrandMA LLM).

![Architecture Diagram](architecture.png)

## Example
Here is a prompt in Bambara, a language spoken in Mali:
```sh
Prompt : Aw ye maana surun dɔ fɔ n ye (kumasen 5 ka caya) waraba ni wulu dɔ kan
Tale : A ko: Waati dɔ, jara dɔ tun be Afiriki jamana na min tɔgɔ ko Sikar. A tun ka fari ani a tun be se ka koo dɔw kɛ. A tun be se ka mɔgɔw bali k'a ka bɛɛn sigi n'a ye. Loon dɔ, k'a to a tagatɔ a ka yɔrɔ kɔlɔsi, a ye wulu dɔ ye. Wuluw tun be siran a ɲɛ. Nka, a hinɛ donna a la, a y'a latigɛ k'a ta k'a kɛ a ka derekeba ye. Wulu nin tɔgɔ ko Timmy. K'a ta o loon na, u kɛra teriw ye. Sikar tun be to ka Timmy kalan a ka dumuni ɲini ani k'a dɛmɛ. U tun be yaala ɲɔgɔn fɛ kongokolon kɔnɔ, ka kongosogow faga ani ka kongosogo farimanw faga. U ka kokɛcogow tun tɛ kelen ye hali dɔɔni.
```