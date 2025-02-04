<script>
    let { img, title, rare, type, name, cor, link} = $props();
    if (type == 'PHY'){
        cor = '#fad81d'
    } else if (type == 'STR'){
        cor = '#f53e3e'
    } else if (type == 'INT'){
        cor = '#c33ef5'
    } else if (type == 'TEQ'){
        cor = '#28ca1b'
    } else {
        cor = '#3ed4f5'
    }
</script>

<div class="card h-100" style="width: 18rem;">
    <img src={img} class="card-img-top" alt="invisibility" width="200px" />
    <div class="card-body" style="background-color: {cor};">
      <h5 class="card-title">{title}</h5>
      <h6 class="card-type">{rare} {type}</h6>
      <p class="card-text">{name}</p>
      <a href="/Dokkan/Card List/{link}" class="btn btn-primary btn-lg active" role="button" aria-pressed="true" style="background-color: orange;"><b>Detalhes</b></a>

    </div>
  </div>

  <style>
    .card-body{
        height: 20%;
    }
    .card {
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.2s ease-in-out;
}

.card:hover {
    transform: scale(1.05);
}

.card-img-top {
    width: 100%;
    height: auto;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
}

.card-body {
    padding: 15px;
    text-align: center;
}

.card-title {
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 5px;
    color: black;
}

.card-type {
    font-size: 1rem;
    color: black;
    margin-bottom: 10px;
}

.card-text {
    font-size: 0.9rem;
    color: black;
    margin-bottom: 15px;
}

.btn-primary {
    background-color: orange !important;
    border: none;
    padding: 10px 15px;
    border-radius: 5px;
    font-weight: bold;
    transition: background 0.3s;
}

.btn-primary:hover {
    background-color: darkorange !important;
}
  </style>