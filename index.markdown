---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<div class="home-container">
    <div class="home-content">
        <h1 class="home-title">{{ site.home.title }}</h1>
        <p class="home-subtitle">{{ site.home.subtitle }}</p>
        <div class="home-buttons">
            {% for button in site.home.buttons %}
            <a href="{{ button.url }}" class="{{ button.type }}-button">{{ button.text }}</a>
            {% endfor %}
        </div>
    </div>
</div>

<div class="about-section">
    <div class="about-container">
        <div class="title-wrapper">
            <img src="/assets/img/quote_mark.svg" alt="Quote Mark" class="quote-mark">
            <h1 class="about-title">{{ site.about.title }}</h1>
        </div>
    </div>
        
    <div class="about-content">
        <div class="about-left">

            <div class="quote-box">
                <img src="/assets/img/small_quote_mark.svg" alt="Quote Mark" class="small-quote-mark">
                <p>{{ site.about.main_quote }}</p>
            </div>
            
            <div class="quote-box">
                <img src="/assets/img/small_quote_mark.svg" alt="Quote Mark" class="small-quote-mark">
                <p>{{ site.about.research_focus }}</p>
            </div>
        </div>
        
        <div class="about-right">
            <div class="quote-box">
                <img src="/assets/img/small_quote_mark.svg" alt="Quote Mark" class="small-quote-mark">
                <p>{{ site.about.join_message }}</p>
                <a href="/join" class="join-button">Join our lab</a>
            </div>
        </div>
    </div>
</div>

<div class="locations-section">

    
    <div class="locations-grid">
        <div class="location-card">
            <img src="/assets/img/hangzhou-location.png" alt="Hangzhou Location">
        </div>
        
        <div class="location-card">
            <img src="/assets/img/beijing-location.png" alt="Beijing Location">
        </div>
        
        <div class="location-card">
            <img src="/assets/img/broad-location.png" alt="Broad Institute Location">
        </div>
    </div>
</div>

<div class="locations-quote">
    <img src="/assets/img/small_quote_mark.svg" alt="Quote Mark" class="small-quote-mark">
    <p>We are physically situated at the <a href="#">Advanced Institute of Information Technology, Peking University</a> in Hangzhou, Zhejiang, <a href="#">School of Public Health, Peking University</a> in Beijing, China and the <a href="#">Broad Institute of MIT and Harvard</a>, Cambridge, MA, US.</p>
</div>

<style>
.title-wrapper {
    position: relative;
}

.quote-mark {
    position: absolute;
    z-index: 0;
    /* 根据需要调整位置和大小 */
}

.about-title {
    position: relative;
    z-index: 1;
}
</style>