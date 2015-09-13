
#Agui van las respuestas

**11.**  la unica manera conocida para deshacer el ultimo commit perdiendo los cambios realizados en el WC
		git reset --hard HEAD~1

**12.**  git reflog  	git reset sha
		porque pienso que es la manera mas comoda y segura de ver que vas al sha coreecto.

**13.**  no, porque htmlify ya estaba updated con la info de master, en otra palabras, ya htmlify tenia todo lo que tenia maaster antes de hacer el merge, era undiferente..

**19.**  si, porque se habia editado en el peom.md de cada rama una info diff pero en lineas con ubicacion similar, y eso causo que git diera el warning.

**21.** yo esparaba un conflicto, pero git no me dio conflicto.. ell merge que hice fue --no-ff, asumo que fue por una condicion similar en el paso 13, pero esperaba el conflicto por la diif de *red* vs *#0000ff*

**25**  como que diduje el diagrama? si el el comando para graph, then git log --graph --decorate --pretty=oneline
  si es literalmente hace el flowchart....

						me di cuenta despues de perder el tiempor que no era esto...




													---------                               
     												       - master  -
       										---------    		----^-----
                                                                     	         - htmlify  -									
                                                                    		 ----^---							 
	---------												-----
      -	matrix	-												HEAD
	----^---												------			
		<-----------------------------------------------------(6)<-----------(7)<------------------(8)
(1)<-------(2) <-------------------------				^				    ^
	    -                            ---------(5)--------------------   <--------------------------------
	    --->(3)-----(4)<--------------	-                         
	 				         -                        
          			   		---------                              
     	        			 	 - htmlify  -              
     	  				        ----^---                  
         
**26.** si, la diff entre ramas es de solo un commit "hay una sola ruta posible.. por asi decirlo"

**27.** intente primero con git --abort pero eso no funciono, entonces --->git reset HEAD~1
**28.** primero git reflog para ver el sha, despues git reset <sha>
**29.** git branch -d
**30.** primero git reflog para ver el sha, despues git reset <sha>, o con ~
**32.** primero git log para ver el sha, luego git checkout <sha>
*33.** primero git log para ver el sha, luego git checkout <sha>
