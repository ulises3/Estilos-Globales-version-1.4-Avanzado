<!--
Autor: Tutorial Blogger
Autor URL: https://blogspot.owinile.com/
Licensia: Creative Commons Attribution 3.0 Unported
Licensia URL: http://creativecommons.org/licenses/by/3.0/
Referencia URL: https://www.zkreations.com/
Referencia URL: http://www.ciudadblogger.com/
-->			

<!-- ETIQUETAS DE DATOS GLOBALES EN BLOGGER --> 

<img expr:src='data:post.firstImageUrl'/> <!-- Primera imagen de la entrada -->	
<img expr:src='data:post.featuredImage'/> <!-- Primera imagen de la entrada canvas.xml v1.9.0 -->	
<expr:alt='data:post.title'/> <!-- Etiqueta ALT para imagenes -->
<data:post.author/>	<!-- Nombre del autor -->	
<data:post.authorProfileUrl/>	<!-- Url del perfil de Blogger o Google+ -->	
<a expr:href='data:post.url' style='color:#fff'></a> <!-- URL hacia la entrada -->	
<data:post.title/> <!-- Título de la entrada -->	
<data:post.date/> <!-- Fecha en el formato configurado -->
<data:post.timestamp/> <!-- Fecha y hora de las entradas en el formato configurado -->
<a expr:href='data:blog.homepageUrl'></a> <!-- URL de la página principal. -->	
<data:blog.title/>	<!-- Título del blog -->
<b:eval expr='data:post.longSnippet snippet {length: 150}'/> <!-- Resumen de la entrada. Máximo 1000 caracteres. No interpreta html -->
<data:post.body/> <!-- Contenido de la entrada. Interpreta Html. -->	
<b:section id='sidebar'> </b:section> <!-- Crear sección sidebar. -->
<data:post.numComments/> <!-- Muestra la cantidad de comentarios. -->
<a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:post.numComments/> Comentarios</a> <!-- Enlace hacia los comentarios.. -->
<a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
 <data:post.numberOfComments/> Comentarios</a> <!-- Enlace hacia los comentarios canvas.xml v1.9.0 -->
<b:loop values='data:post.labels' var='label'><a expr:href='data:label.url'><data:label.name/></a></b:loop> <!-- Muestra variable label expresada en un bucle. -->
<data:blog.metaDescription/> <!-- Muestra la meta descripcion de la página o del post. -->
<form expr:action='data:blog.searchUrl'> <!-- Ejecuta el enlace de la pagina de busqueda. -->
<input name='q' expr:value='data:view.isSearch ? data:view.search.query.escaped : &quot;&quot;' /> <!-- Devuelve la busqueda en el blog. -->
<input expr:value='data:messages.search'/> <!-- Muestra el boton "Buscar". -->
<URL-de-mi-blog/search?max-results=1000> <!-- Muestra la página de resultados para las busquedas". -->
<expr:style='&quot;background-image: url(&quot; + data:blog.postImageUrl + &quot;);&quot;'/> <!-- Muestra la primera imagen del post como background -->	
	

	

<!-- CONDICIONALES DE BLOGGER --> 

<b:if cond='data:blog.homepageUrl == data:blog.url'> <!-- Mostrar gadgets solo en la portada -->	
<b:if cond='data:blog.pageType == &quot;item&quot;'> <!-- Ejecutar un elemento sólo en las entradas individuales -->
<b:if cond='data:blog.pageType == &quot;archive&quot;'> <!-- Ejecutar un elemento en las páginas del archivo -->
<b:if cond='data:blog.pageType == &quot;static_page&quot;'> <!-- Ejecutar elemento en las páginas estáticas -->  
<b:if cond='data:blog.url == &quot;URL de la entrada o etiqueta&quot;'>  <!-- Ejecutar elemento en una entrada específica o etiqueta específica -->
<b:if cond='data:blog.url != data:blog.homepageUrl'> <!-- Ejecutar un elemento en todas las páginas MENOS en la portada del blog --> 
<b:if cond='data:blog.pageType != &quot;item&quot;'> <!-- Ejecutar elemento en todas las páginas MENOS en las entradas individuales -->
<b:if cond='data:blog.pageType != &quot;archive&quot;'> <!-- Ejecutar elemento en todas las páginas MENOS en las páginas del archivo del blog -->   
<b:if cond='data:blog.pageType != &quot;static_page&quot;'> <!-- Ejecutar elemento en todas las páginas MENOS en las páginas estáticas -->   
<b:if cond='data:blog.url != &quot;URL de la entrada o etiqueta&quot;'> <!-- Ejecutar  en todas las páginas MENOS en una entrada específica o etiqueta específica -->   
<b:if cond='data:view.isError'><!-- url no existe muestra la pagina de error 404-->
<b:else/> <!-- casos contrario muestra el blog-->
</b:if> <!-- Cierre de la condicional -->
<b:attr cond='not data:view.isPreview' name='target' value='_top'/> <!-- Condición que indica que no es una vista previa. -->
<b:if cond='data:view.isSearch'> <!-- Mostrar gadgets solo en la página de resutados para la busqueda -->

 
