<template>
    <div class="proyectos">
       <!---->
        <!--Inicia formulario form-->
              
              
        <div>
        <el-container>
                    <el-aside width="200px" style="color: #EAF2E3"><h1>MENU</h1>
                    <el-button slot="append" icon="el-icon-search"></el-button>
                     <!-- ======================cascada====================== -->
                      <el-cascader
                        :options="options"
                        :show-all-levels="false"
                    ></el-cascader>
                    <!-- ======================botones====================== -->
                      <el-button type="primary">Top Proyectos</el-button>
                        <el-button type="primary">Mas Recientes</el-button>
                          <el-button type="primary">Nuevas Versiones</el-button>
                    </el-aside>
            <el-container>
                <el-header style="color: #303133"><h2>PROYECTOS EXISTENTES</h2></el-header>
                    <!-- ======================inicio del main====================== -->
                    <el-main>
                      <!-- 
                        <div style="margin-top: 15px;">
                        <el-input placeholder="Buscar en Categoria" v-model="input5" class="input-with-select">
                            <el-select v-model="select" slot="prepend" placeholder="Select">
                                <el-option label="Navegadores y Sistemas Operativos" value="Navegadores y Sistemas Operativos"></el-option>
                                <el-option label="Plataformas móviles" value="Plataformas móviles"></el-option>
                                <el-option label="Lenguajes de programación" value="Lenguajes de programación"></el-option>
                                <el-option label="Aplicaciones de trabajo" value="Aplicaciones de trabajo"></el-option>
                            </el-select>
                            <el-button slot="append" icon="el-icon-search"></el-button>
                        </el-input>
                        </div>-->
                        <div>

                          
                        </div>
                        <el-row>
                          <el-col :span="8"><div class="grid-content bg-purple">
                              <H1>Wordpress: https://wordpress.org/</h1> 
                        <H1>Ubuntu  https://www.ubuntu.com/</h1>   
                        <H1>Notepad  https://notepad-plus-plus.org/</h1> 
                        <H1>Linux https://www.linux.org/</h1> 
                        <H1>NetBeans https://netbeans.org/</h1> 
                        <H1>Eclipse https://www.eclipse.org/</h1> 
                         <H1>Junit https://junit.org/junit5/</h1> 
                        <H1>PMD https://pmd.github.io/</h1> 
                            </div></el-col>

                          <el-col :span="8"><div class="grid-content bg-purple-light">
                             <H1>Hibernate http://hibernate.org/</h1> 
                        <H1>SQLite https://www.sqlite.org/index.html</h1> 
                        <H1>MySQL https://www.mysql.com/</h1> 
                        <H1>Apache Derby https://db.apache.org/derby/</h1> 
                        <H1>Valgrind http://valgrind.org/</h1> 
                        <H1>Audacity https://sourceforge.net/projects/audacity/</h1> 
                        <H1>Videolan http://www.videolan.org/</h1> 
                        <H1>Postgresql https://www.postgresql.org/</h1> 
                         <H1>Apache Cordova http://cordova.apache.org/</h1> 
                            </div></el-col>
                          <el-col :span="8"><div class="grid-content bg-purple">
                        <H1>FFmpeg https://ffmpeg.org/</h1> 
                        <H1>Velocity https://velocity.apache.org/</h1> 
                        <H1>Freetype https://www.freetype.org/</h1> 
                        <H1>jQuery https://jquery.com/</h1> 
                        <H1>Kubernetes https://kubernetes.io/</h1> 
                        <H1>Docker https://www.docker.com/</h1> 
                        <H1>Nodejs https://nodejs.org/es/</h1> 
                        <H1>Apache Sparks https://spark.apache.org/</h1> 
                            </div></el-col>
                        </el-row>
                      
                       
                       
                        
                    </el-main>
                    <!-- ======================fin del main====================== -->
                <el-footer style="color: #303133"><h2> </h2>
                
                
                </el-footer>
            
            </el-container>
        </el-container>
 
        </div>


    </div>
</template>


<script>
import EditableCell from "./EditableCell.vue";
export default {
     data() {
       show3: true
    return {
      input1: '',
      input2: '',
      input3: '',
      input4: '',
      input5: '',
      select: ''
    }
  },
    //este es el botton de seleccionar categoria en cascada
  data() {
      return {
        options: [{
            //LABEL ES EL NOMBRE DE CATEGORIA
            //======================rama1======================
          value: 'guide',
          label: 'Herramientas de Desarrollo Web Frontend', 
          children: [{
            value: 'bootstrap',
            label: 'Bootstrap',
            }, {
            value: 'jquery',
            label: 'jQuery',
            },
             {
            value: 'apache',
            label: 'Apache Cordova',
            }, {
            value: 'backbone',
            label: 'Backbone',
            }, {
            value: 'angular',
            label: 'AngularJS',
            }, {
            value: 'javascript',
            label: 'Javascript',
          
          }],
          
        }, {
            //  =======================rama2======================
          value: 'form',
          label: 'Herramientas de Desarrollo Web Backend',
          children: [{
            value: 'php',
            label: 'PHP',
            }, {
            value: 'java',
            label: 'Java',
            }, {
            value: 'ruby',
            label: 'Ruby',
            }, {
            value: 'python',
            label: 'Python',
            }, {
            value: 'node',
            label: 'NodeJS',
            }]
        }, {
            //======================rama3======================
          value: 'navigation',
          label: 'Sistemas de Gestión de Contenidos',
          children: [{
            value: 'wordpress',
            label: 'Wordpress',
            }, {
            value: 'prestashop',
            label: 'Prestashop',
            }, {
            value: 'joomla',
            label: 'Joomla',
            }, {
            value: 'drupal',
            label: 'Drupal',
            }],
          
        }, {
            //  =======================rama4======================
          value: 'resource',
          label: 'Bases de Datos',
          children: [{
            value: 'maria',
            label: 'MariaDB',
            }, {
            value: 'redis',
            label: 'Redis',
            }, {
            value: 'postgre',
            label: 'PostgreSQL',
            }, {
            value: 'my',
            label: 'MySQL',
            }, {
            value: 'mongo',
            label: 'MongoDB',
            }, {
            value: 'sqlite',
            label: 'SQLite',
            }]
        }, {
            //======================rama5======================
          value: 'components',
          label: 'Herramientas DevOps',
          children: [{
            value: 'docker',
            label: 'Docker'
          }, {
            value: 'openstack',
            label: 'Drone.io'
          }, {
            value: 'kubernetes',
            label: 'Kubernetes'
          }, {
            value: 'cloud',
            label: 'Django'
          }]
        }]
      };
    },
  
name: 'proyectos',
  components: {
    EditableCell
    }
    
    }
    
</script>


<style>
.el-header, .el-footer {
    background-color: #f4f1bb;
    color: #333;
    text-align: center;
    line-height: 60px;
  }
  
  .el-aside {
    background-color: rgb(159, 214, 236);
    color: #333;
    text-align: center;
    line-height: 100px;
  }
  
  .el-main {
    background-color: #FDFDF0;
    color: #333;
    text-align: center;
    line-height: 90px;
  }

   
</style>
