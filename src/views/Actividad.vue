<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <ActividadController :cuestionario="cuestionario"/>
  
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Propuesta comercial de un producto o servicio',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> apropiarse de los conocimientos asociados a la propuesta comercial de un producto o servicio, así mismo las técnicas de negociación y herramientas para la socialización de esta.',
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      barajarPreguntas: false,
      preguntas: [
        {
          id: 1,
          texto: '¿Qué busca satisfacer una propuesta comercial?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Los objetivos financieros de la empresa únicamente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Las necesidades y deseos de los clientes.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Las exigencias de los proveedores.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Las regulaciones gubernamentales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 2,
          texto: '¿Qué es un producto?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Una estrategia de ventas.', esCorrecta: false },
            { id: 'b', texto: 'Un proceso administrativo.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Un bien o servicio que satisface una necesidad o deseo.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Un canal de distribución.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 3,
          texto:
            '¿Cuál de los siguientes elementos forma parte de la presentación física de un producto?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Publicidad.', esCorrecta: false },
            { id: 'b', texto: 'Promoción.', esCorrecta: false },
            { id: 'c', texto: 'Garantía.', esCorrecta: false },
            { id: 'd', texto: 'Empaque.', esCorrecta: true },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 4,
          texto: '¿Qué función cumple la etiqueta de un producto?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Proporcionar información relevante sobre el producto.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Aumentar el costo del producto.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Sustituir el empaque.', esCorrecta: false },
            { id: 'd', texto: 'Controlar la distribución.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 5,
          texto: '¿Qué es el embalaje?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El diseño gráfico de una marca.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'El precio de venta del producto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La protección externa utilizada para almacenar y transportar productos.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'La promoción del producto.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 6,
          texto: '¿Qué son los atributos de un producto?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Los canales de distribución.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Las características que permiten diferenciarlo de otros productos.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Las estrategias de negociación.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Los costos de producción.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 7,
          texto: '¿Qué representan los niveles de un producto?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La cantidad de ventas obtenidas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La clasificación de clientes.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Los beneficios básicos, reales y aumentados que ofrece al consumidor.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Los procesos de fabricación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 8,
          texto: '¿Cuál es una característica de un producto de calidad?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Genera mayores costos.', esCorrecta: false },
            { id: 'b', texto: 'Tiene menor duración.', esCorrecta: false },
            { id: 'c', texto: 'Presenta poca utilidad.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Satisface las expectativas del consumidor.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 9,
          texto: '¿Qué es el servicio al cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Una técnica de publicidad.', esCorrecta: false },
            { id: 'b', texto: 'Un método de producción.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'El conjunto de actividades orientadas a atender y satisfacer al cliente.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Un canal de distribución.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 10,
          texto: '¿Cuál es un atributo importante del servicio al cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Demora en la atención.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Amabilidad y disposición para ayudar.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Incremento de precios.', esCorrecta: false },
            { id: 'd', texto: 'Reducción de beneficios.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 11,
          texto:
            '¿Cuál es una característica de un excelente servicio al cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Falta de comunicación.', esCorrecta: false },
            { id: 'b', texto: 'Atención limitada.', esCorrecta: false },
            { id: 'c', texto: 'Escasa disponibilidad.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Rapidez y eficiencia en la respuesta.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 12,
          texto: '¿Qué es el surtido de productos?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'El conjunto de productos que una empresa ofrece a sus clientes.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'El precio de una línea de productos.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'El diseño del empaque.', esCorrecta: false },
            { id: 'd', texto: 'El proceso de negociación.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 13,
          texto: '¿Qué se entiende por la estructura del surtido?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El diseño del establecimiento.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La distribución de clientes.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La organización de los productos dentro de las diferentes categorías.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'La estrategia publicitaria.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 14,
          texto: '¿Qué permite la clasificación del surtido?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Aumentar los precios.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Organizar los productos según características comunes.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Reducir el inventario.', esCorrecta: false },
            { id: 'd', texto: 'Eliminar categorías.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 15,
          texto: '¿Qué se entiende por dimensiones del surtido?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El tamaño físico del almacén.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'El número de empleados.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'La amplitud, profundidad y longitud de las líneas de productos.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'La cantidad de proveedores.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 16,
          texto: '¿Cuál es una cualidad deseable en un surtido?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Escasa variedad.', esCorrecta: false },
            { id: 'b', texto: 'Productos desactualizados.', esCorrecta: false },
            { id: 'c', texto: 'Baja disponibilidad.', esCorrecta: false },
            {
              id: 'd',
              texto:
                'Capacidad de responder a las necesidades de diferentes clientes.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 17,
          texto: '¿Qué es la negociación?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Un proceso de fabricación.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Un sistema de distribución.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Un proceso de comunicación para llegar a acuerdos entre dos o más partes.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Un método de publicidad.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 18,
          texto: '¿Cuál es una etapa de la negociación?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Preparación.', esCorrecta: true },
            { id: 'b', texto: 'Producción.', esCorrecta: false },
            { id: 'c', texto: 'Distribución.', esCorrecta: false },
            { id: 'd', texto: 'Facturación.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 19,
          texto:
            '¿Cuál es el propósito principal de las herramientas ofimáticas en una propuesta comercial?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Diseñar productos.', esCorrecta: false },
            { id: 'b', texto: 'Transportar mercancías.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'Facilitar la creación, organización y presentación de información.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Realizar procesos de manufactura.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
        {
          id: 20,
          texto: '¿Cuál de las siguientes es una herramienta ofimática?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Máquina industrial.', esCorrecta: false },
            { id: 'b', texto: 'Vehículo de carga.', esCorrecta: false },
            { id: 'c', texto: 'Calculadora científica.', esCorrecta: false },
            { id: 'd', texto: 'Procesador de texto.', esCorrecta: true },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de la Propuesta comercial de un producto o servicio.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Propuesta comercial de un producto o servicio.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
  computed: {},
  methods: {},
}
</script>
