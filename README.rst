cne
===

.. image:: https://img.shields.io/pypi/v/cne.svg?style=flat-square
    :target: https://pypi.python.org/pypi/cne

.. image:: https://img.shields.io/pypi/dm/cne.svg?style=flat-square
    :target: https://pypi.python.org/pypi/cne

.. image:: https://img.shields.io/pypi/wheel/cne.svg?style=flat-square
    :target: https://pypi.python.org/pypi/cne

.. image:: https://img.shields.io/pypi/format/cne.svg?style=flat-square
    :target: https://pypi.python.org/pypi/cne

.. image:: https://img.shields.io/pypi/pyversions/cne.svg?style=flat-square
    :target: https://pypi.python.org/pypi/cne

.. image:: https://img.shields.io/pypi/status/cne.svg?style=flat-square
    :target: https://pypi.python.org/pypi/cne

.. image:: https://img.shields.io/pypi/l/cne.svg?style=flat-square
    :target: https://raw.githubusercontent.com/lgaticaq/python-cne/master/LICENSE

.. image:: https://img.shields.io/travis/lgaticaq/python-cne.svg?style=flat-square
    :target: https://travis-ci.org/lgaticaq/python-cne

.. image:: https://img.shields.io/badge/gitter-join%20chat%20%E2%86%92-brightgreen.svg?style=flat-square
    :target: https://gitter.im/lgaticaq/python-cne?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge

Get fuel price from cne api

Installation
------------

.. code-block:: bash

    $ pip install cne


Use
---

.. code-block:: python

    >>> import cne
    >>> data = cne.get(fuelType='gasolina_95', commune='santiago')
    >>> print(data)
    {
        id: 'ul1510101',
        fecha: '2015-07-24 20:29:23',
        direccion_calle: 'Barros Arana',
        direccion_numero: '3081',
        latitud: -18.458676528284,
        longitud: -70.288939476013,
        nombre_comuna: 'Arica',
        nombre_distribuidor: 'Uligas',
        tienda_conveniencia: '',
        farmacia: '',
        bano_publico: '1',
        servicios_mantencion: '',
        autoservicio: '',
        horario_atencion: 'HH',
        precio_por_combustible: {
          glp_vehicular: 393
        },
        metodos_de_pago: {
          efectivo: '1'
        }
    }

Fuel types availables
---------------------

.. code-block:: bash

    gasolina_93, gasolina_95, gasolina_97, glp_vehicular, gnc, kerosene, petroleo_diesel


Communes availables
-------------------

.. code-block:: bash

    Aisén, Algarrobo, Alhué, Alto Hospicio, Ancud, Andacollo, Angol, Antofagasta, Antuco, Arauco, Arica, Buin, Bulnes, Cabildo, Cabo de Hornos, Cabrero, Calama, Calbuco, Caldera, Calera de Tango, Calera, Calle Larga, Canela, Carahue, Cartagena, Casablanca, Castro, Catemu, Cauquenes, Cañete, Cerrillos, Cerro Navia, Chaitén, Chanco, Chañaral, Chiguayante, Chile Chico, Chillán Viejo, Chillán, Chimbarongo, Cholchol, Chonchi, Chépica, Cisnes, Cobquecura, Cochamó, Cochrane, Coelemu, Coihaique, Coihueco, Colbún, Colina, Collipulli, Coltauco, Combarbalá, Concepción, Conchalí, Concón, Constitución, Contulmo, Copiapó, Coquimbo, Coronel, Corral, Cunco, Curacautín, Curacaví, Curanilahue, Curarrehue, Curepto, Curicó, Dalcahue, Diego de Almagro, Doñihue, El Bosque, El Carmen, El Monte, El Quisco, Empedrado, Ercilla, Estación Central, Florida, Freire, Fresia, Frutillar, Futrono, Galvarino, Gorbea, Graneros, Guaitecas, Hijuelas, Hualaihué, Hualañé, Hualpén, Huasco, Huechuraba, Illapel, Independencia, Iquique, Isla de Maipo, Isla de Pascua, La Cisterna, La Cruz, La Estrella, La Florida, La Granja, La Ligua, La Pintana, La Reina, La Serena, La Unión, Lago Ranco, Laja, Lampa, Lanco, Las Cabras, Las Condes, Lautaro, Lebu, Licantén, Limache, Linares, Litueche, Llaillay, Llanquihue, Lo Barnechea, Lo Espejo, Lo Prado, Lolol, Loncoche, Longaví, Lonquimay, Los Andes, Los Lagos, Los Muermos, Los Sauces, Los Vilos, Los Álamos, Los Ángeles, Lota, Lumaco, Machalí, Macul, Maipú, Malloa, Marchihue, Mariquina, María Elena, María Pinto, Maule, Maullín, Mejillones, Melipeuco, Melipilla, Molina, Monte Patria, Mostazal, Mulchén, Máfil, Nacimiento, Nancagua, Natales, Navidad, Negrete, Ninhue, Nogales, Nueva Imperial, Ñiquén, Ñuñoa, Olivar, Olmué, Osorno, Ovalle, OHiggins, Padre Hurtado, Padre las Casas, Paillaco, Paine, Palena, Palmilla, Panguipulli, Panquehue, Papudo, Paredones, Parral, Pedro Aguirre Cerda, Pelarco, Pelluhue, Pemuco, Pencahue, Penco, Peralillo, Perquenco, Petorca, Peumo, Peñaflor, Peñalolén, Pica, Pichidegua, Pichilemu, Pinto, Pirque, Pitrufquén, Placilla, Porvenir, Pozo Almonte, Primavera, Providencia, Puchuncaví, Pucón, Pudahuel, Puente Alto, Puerto Montt, Puerto Octay, Puerto Varas, Pumanque, Punitaqui, Punta Arenas, Purranque, Purén, Putaendo, Puyehue, Queilén, Quellón, Quilicura, Quillota, Quillón, Quilpué, Quinchao, Quinta Normal, Quinta de Tilcoco, Quintero, Quirihue, Rancagua, Rauco, Recoleta, Renaico, Renca, Rengo, Requínoa, Retiro, Rinconada, Romeral, Ránquil, Río Bueno, Río Claro, Río Ibáñez, Río Negro, Saavedra, Sagrada Familia, Salamanca, San Antonio, San Bernardo, San Carlos, San Clemente, San Esteban, San Felipe, San Fernando, San Gregorio, San Ignacio, San Javier, San Joaquín, San José de Maipo, San Miguel, San Nicolás, San Pablo, San Pedro de Atacama, San Pedro de la Paz, San Rafael, San Ramón, San Vicente, Santa Bárbara, Santa Cruz, Santa Juana, Santa María, Santiago, Santo Domingo, Sierra Gorda, Talagante, Talca, Talcahuano, Taltal, Temuco, Teno, Teodoro Schmidt, Tierra Amarilla, Tiltil, Tirúa, Tocopilla, Toltén, Tomé, Traiguén, Tucapel, Valdivia, Vallenar, Valparaíso, Victoria, Vicuña, Vilcún, Villa Alegre, Villa Alemana, Villarrica, Vitacura, Viña del Mar, Yerbas Buenas, Yumbel, Yungay, Zapallar


Distributors availables
-----------------------

.. code-block:: bash

    ABASTIBLE, APEX, ATT, AUTOGASCO, BALTOLU, CAVE, CHILIN, COC, COMBUSTIBLES AMADE, COMBUSTIBLES JCD, COMERCIAL MAQUI, COPEC, CUSTOM SERVICE, Combustible Alhue, Combustibles Endless.com, Combustibles Ortiz, Coopeserau, Cremaschi, DELPA, ECCO, ECOGREEN LTDA., EL HUIQUE, ENERSUR S.A., FACAZ, HN, HOLA!, J Allel, JLC, LIDER S.A., LIPIGAS, PETROBRAS, PETROJAC, PETRONEXT, Puma Verde, Rafael Letelier Yañez y Cia Ltda, SERVICENTRO LEAL, SERVICENTRO SAN MIGUEL, SERVICENTROS RABALME, SESA, SHELL, SINHEL, SOCORRO, SUAREZ COMBUSTIBLES, SURENERGY, Sin Bandera, TERPEL, Uligas, VIVA COMBUSTIBLES
