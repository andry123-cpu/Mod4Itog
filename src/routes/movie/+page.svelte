
<style>
    :root {
    --primary-color: rgb(41, 52, 39);
    --secodary-color: rgb(26, 217, 255);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}

body{
    background-color:  var(--primary-color);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
}

header {
    padding: 10px;
    display: flex;
    justify-content: flex-end;
    background-color: var(--secodary-color);
}

.search {
    background-color: transparent;
    border: 2px solid var(--primary-color);
    border-radius: 50px;
    font-family: inherit;
    font-size: 14px;
    padding: 20px 10px;
}

.search::placeholder {
    color: wheat;
}

.search.search:focus{
    outline: none;
    background-color: white;
}

.movie {
    width: 3000px;
    margin: 30px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.movie img{
    width: 100%;
}

.movie-info {
    color: black;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 40px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: lightgreen;
}

.overview {
    background-color: white;
    padding: 7px;
    position: absolute;
    text-decoration-color: aliceblue;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}
</style>

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Адам и Ева</h3>
            <span class="green">9.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">Романтическая комедия, Марина и Виктор - остались единственными людьми в огромном городе...</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Первая дуэль</h3>
            <span class="green">8.0</span>
        </div>
        <div class="overview">
            <h3 id="Description">Драма, исторически, Экшен; Париж 1887 год. Время когда дороже всего ценилась дуэль...</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Демоны дома Гарретов</h3>
            <span class="green">7.9</span>
        </div>
        <div class="overview">
            <h3 id="Description">Хоррор, триллер: Джой - Неле гальная иммигрантка, которая берётся...  </h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Лёд 3</h3>
            <span class="green">9.0</span>
        </div>
        <div class="overview">
            <h3 id="Description">Мелодрама: Надя выросла и стала фигуристкой. Она мечтает о... </h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Позывной "Пассажир"</h3>
            <span class="green">9.7</span>
        </div>
        <div class="overview">
            <h3 id="Description">Драмма: Молодой писатель живёт в столице, проводит время в... </h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Валентина</h3>
            <span class="green">7.0</span>
        </div>
        <div class="overview">
            <h3 id="Description">Анимация: Девочка хочет стать гимнасткой и для этого... </h3>
        </div>
    </div>

</main>