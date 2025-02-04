<script>
    let { children } = $props();
</script>
<div class="body" style="background-color: lightgreen;">
<nav class="navbar navbar-expand-sm bg-body-tertiary">
    <div class="container-fluid">
        <a class="navbar-brand" href="/#">
            <img src="/iconedokkan.png" alt="Logo" width="24" height="24" />
            Dokkan Battle Card List
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a class="nav-link" href="/#">Página Inicial</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/Dokkan/Card List">Lista de personagens</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/Dokkan/Sobre o criador">Sobre mim</a>
                </li>
            </ul>
        </div>
    </div>
</nav>
</div>
<style>
.navbar {
    background-color: darkgreen !important;
    padding: 10px 20px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.navbar-brand {
    font-size: 1.5rem;
    font-weight: bold;
    color: #ecf0f1 !important;
    display: flex;
    align-items: center;
    gap: 8px;
}

.navbar-brand img {
    border-radius: 50%;
}

.navbar-toggler {
    border: none;
}

.navbar-toggler-icon {
    filter: invert(100%);
}

.navbar-nav {
    margin-left: auto;
}

.nav-item {
    margin: 0 10px;
}

.nav-link {
    font-size: 1rem;
    color: #ecf0f1 !important;
    transition: color 0.3s;
}

.nav-link:hover {
    color: #f39c12 !important;
}

</style>
{@render children()}
