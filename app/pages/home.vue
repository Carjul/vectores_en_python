<template>
  <div class="navbar bg-base-100">
    <div class="flex-none">
      <button class="btn btn-square btn-ghost">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
          class="inline-block w-5 h-5 stroke-current">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
        </svg>
      </button>
    </div>
    <div class="flex-1">
      <NuxtLink class="btn btn-ghost normal-case text-xl" to="/">Inicio</NuxtLink>

    </div>
    <div class="flex-none">
      <button class="btn btn-square btn-ghost">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24"
          class="inline-block w-5 h-5 stroke-current">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z">
          </path>
        </svg>
      </button>
    </div>
  </div>


  <div className="flex justify-center items-center mt-20 ">
    <div className=" card w-4/5 h-auto bg-base-100 shadow-xl">

      <div className="card-body">
        <h1 className="card-title justify-center mt-2">Vectore en Python</h1>
        <br>
        <p className="p-4">En Python, un vector generalmente se refiere a una secuencia unidimensional de elementos,
          similar a lo que se conoce como una lista o array unidimensional. Los vectores se utilizan para almacenar y
          manipular datos de una manera estructurada y eficiente. Los vectores son una parte fundamental en la
          programación y se utilizan en una variedad de contextos, desde cálculos matemáticos hasta manipulación de datos
        </p>
        <figure class="mb-10"><img
            src=" data:image/png;base64,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"
            alt="Shoes" /></figure>

      </div>
    </div>
  </div>

  <div className="flex justify-center items-center mt-20 ">
    <div className=" card w-4/5 h-auto bg-base-100 shadow-xl">

      <div className="card-body">
        <h1 className="card-title justify-center mt-2">NUMPY - Vectores y Matrices</h1>
        <br>
        <p className="p-4">NumPy es una libreria de Algebra Lineal para Python, la razón por la cual es tan importante
          para Data Science con Python es que casi todas las librerias del ecosistema de PyData confían en NumPy como uno
          de sus principales componentes.

          Numpy también es increíblemente rápido, ya que tiene enlaces a librerias en C. Para obtener más información
          sobre por qué usar Arrays en lugar de listas
        </p>
        <h2 className="card-title justify-center mt-2">Importando NumPy</h2>
        <br>
        <figure class="mb-10">
          <div class="mockup-code">
            <pre data-prefix="$"><code># esta es la forma estandar de importar numpy</code></pre>
            <pre data-prefix=">" class="text-warning"><code>import numpy as np </code></pre>
          </div>
        </figure>

      </div>
    </div>
  </div>

  <div className="flex justify-center items-center mt-20 ">
    <div className=" card w-4/5 h-auto bg-base-100 shadow-xl">

      <div className="card-body">
        <h1 className="card-title justify-center mt-2">Arreglos en Numpy (Arrays)</h1>
        <br>
        <p className="p-4">Los arreglos en NumPy son la principal forma de usar Numpy. Los arreglos de NumPy esencialmente
          vienen en dos tipos: vectores y matrices. Los vectores son estrictamente matrices de 1-d y las matrices son 2-d
          (pero debe tener en cuenta que una matriz aún puede tener solo una fila o una columna).
        </p>
        <h2 className="card-title justify-center mt-2">Crear Arreglos desde Listas de Python</h2>
        <br>
        <figure class="mb-10">
          <div class="mockup-code">
            <pre data-prefix="$"><code>#lista en python</code></pre>
            <pre data-prefix="$"><code>my_list = [1,2,3] </code></pre>
            <pre data-prefix="$"><code>#Convertir lista a vector</code></pre>
            <pre data-prefix=">" class="text-warning"><code>np.array(my_list) </code></pre>
          </div>
        </figure>
        <br>
        <figure class="mb-10">
          <div class="mockup-code">
            <pre data-prefix="$"><code>my_matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] # Una lista de listas </code> </pre>
            <pre data-prefix="$"><code>np.array(my_matrix) # conversion de una lista de listas a Matriz</code></pre>
            <pre data-prefix=">"
              class="text-warning"><code>array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]) #resultado</code></pre>

          </div>
        </figure>
      </div>
    </div>
  </div>

  <div className="flex justify-center items-center mt-20">
  <div className="card w-4/5 h-auto bg-base-100 shadow-xl">

    <div className="card-body">
      <h1 className="card-title justify-center mt-2">NUMPY - Vectores y Matrices</h1>

      <div className="p-4">
        <p>
          NumPy es una librería de Álgebra Lineal para Python. La razón por la cual es tan importante para Data Science con Python es que casi todas las librerías del ecosistema de PyData confían en NumPy como uno de sus principales componentes.
        </p>

        <p>
          Numpy también es increíblemente rápido, ya que tiene enlaces a librerías en C. Para obtener más información sobre por qué usar Arrays en lugar de listas.
        </p>

        <h2 className="card-title justify-center mt-2">Métodos integrados (Built-in Methods)</h2>

        <p>
          Existen muchas funciones para generar arreglos:
        </p>

        <div className="mockup-code">
          <pre data-prefix="$"><code>arange</code>: Devuelve valores espaciados uniformemente dentro de un intervalo dado. Es muy parecida a la función <code>range</code> de las básicas de Python.</pre>
          <pre data-prefix="$"><code>np.arange(0, 10)  # arange(valor_inicial, valor_final-1)</code></pre>
          <pre data-prefix="$"><code>np.arange(0, 11, 2)  # arange(valor_inicial, valor_final-1, paso)</code></pre>
          <pre data-prefix="$"><code>zeros</code> y <code>ones</code>: Generan arreglos de Ceros o Unos.</pre>
          <pre data-prefix="$"><code>np.zeros(3)  # Generar un arreglo de ceros que contenga 3 elementos</code></pre>
          <pre data-prefix="$"><code>np.zeros((5, 5))  # Generar una matriz de ceros de 5 x 5 elementos</code></pre>
          <pre data-prefix="$"><code>np.ones(3)  # Generar un arreglo de unos que contenga 3 elementos</code></pre>
          <pre data-prefix="$"><code>np.ones((3, 3))  # Generar una matriz de unos de 3 x 3 elementos</code></pre>
        </div>
      </div>
    </div>
  </div>
</div>



  <div className="flex justify-center items-center mt-20">
    <div className="card w-full md:w-4/5 bg-base-100 shadow-xl">
      <div className="card-body">
        <h1 className="card-title text-center mt-2">Video de Vectores</h1>
        <div className="p-4">
          <div class="mx-auto">
            <iframe width="90%" height="450" src="https://www.youtube.com/embed/BwW3t17wt5E?si=QZ1vK0pMeGg10NMH"
              title="YouTube video player" frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen></iframe>
          </div>
        </div>
      </div>
  </div>
</div></template>