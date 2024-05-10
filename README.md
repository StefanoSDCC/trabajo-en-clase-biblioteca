public class Usuario {
    private String nombre;
    private String dni;
    private String direccion;

    public Usuario(String nombre, String dni, String direccion) {
        this.nombre = nombre;
        this.dni = dni;
        this.direccion = direccion;
    }

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public String getDni() {
        return dni;
    }

    public void setDni(String dni) {
        this.dni = dni;
    }

    public String getDireccion() {
        return direccion;
    }

    public void setDireccion(String direccion) {
        this.direccion = direccion;
    }

    @Override
    public String toString() {
        return "Usuario{" +
                "nombre='" + nombre + '\'' +
                ", dni='" + dni + '\'' +
                ", direccion='" + direccion + '\'' +
                '}';
    }
}

public class Revista {
    private String titulo;
    private String editor;
    private String categoria;
    private String periodicidad;
    private String ISSN;

    public Revista(String titulo, String editor, String categoria, String periodicidad, String ISSN) {
        this.titulo = titulo;
        this.editor = editor;
        this.categoria = categoria;
        this.periodicidad = periodicidad;
        this.ISSN = ISSN;
    }

    public String getTitulo() {
        return titulo;
    }

    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public String getEditor() {
        return editor;
    }

    public void setEditor(String editor) {
        this.editor = editor;
    }

    public String getCategoria() {
        return categoria;
    }

    public void setCategoria(String categoria) {
        this.categoria = categoria;
    }

    public String getPeriodicidad() {
        return periodicidad;
    }

    public void setPeriodicidad(String periodicidad) {
        this.periodicidad = periodicidad;
    }

    public String getISSN() {
        return ISSN;
    }

    public void setISSN(String ISSN) {
        this.ISSN = ISSN;
    }

    @Override
    public String toString() {
        return "Revista{" +
                "titulo='" + titulo + '\'' +
                ", editor='" + editor + '\'' +
                ", categoria='" + categoria + '\'' +
                ", periodicidad='" + periodicidad + '\'' +
                ", ISSN='" + ISSN + '\'' +
                '}';
    }
}

public class Libro {
    private String titulo;
    private String autor;
    private String isbn;
    private int numPaginas;

    public Libro(String titulo, String autor, String isbn, int numPaginas) {
        this.titulo = titulo;
        this.autor = autor;
        this.isbn = isbn;
        this.numPaginas = numPaginas;
    }

    public String getTitulo() {
        return titulo;
    }

    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public String getAutor() {
        return autor;
    }

    public void setAutor(String autor) {
        this.autor = autor;
    }

    public String getIsbn() {
        return isbn;
    }

    public void setIsbn(String isbn) {
        this.isbn = isbn;
    }

    public int getNumPaginas() {
        return numPaginas;
    }

    public void setNumPaginas(int numPaginas) {
        this.numPaginas = numPaginas;
    }

    @Override
    public String toString() {
        return "Libro{" +
                "titulo='" + titulo + '\'' +
                ", autor='" + autor + '\'' +
                ", isbn='" + isbn + '\'' +
                ", numPaginas=" + numPaginas +
                '}';
    }
}

public class Periodico {
    private String titulo;
    private String editor;
    private String seccion;
    private String fechaPublicacion;

    public Periodico(String titulo, String editor, String seccion, String fechaPublicacion) {
        this.titulo = titulo;
        this.editor = editor;
        this.seccion = seccion;
        this.fechaPublicacion = fechaPublicacion;
    }

    public String getTitulo() {
        return titulo;
    }

    public void setTitulo(String titulo) {
        this.titulo = titulo;
    }

    public String getEditor() {
        return editor;
    }

    public void setEditor(String editor) {
        this.editor = editor;
    }

    public String getSeccion() {
        return seccion;
    }

    public void setSeccion(String seccion) {
        this.seccion = seccion;
    }

    public String getFechaPublicacion() {
        return fechaPublicacion;
    }

    public void setFechaPublicacion(String fechaPublicacion) {
        this.fechaPublicacion = fechaPublicacion;
    }

    @Override
    public String toString() {
        return "Periodico{" +
                "titulo='" + titulo + '\'' +
                ", editor='" + editor + '\'' +
                ", seccion='" + seccion + '\'' +
                ", fechaPublicacion='" + fechaPublicacion + '\'' +
                '}';
    }
}

public class Main {
    public static void main(String[] args) {
        // Crear un objeto Usuario
        Usuario usuario = new Usuario("Juan Pérez", "12345678A", "Calle Principal 123");
        System.out.println("Información del Usuario:");
        System.out.println(usuario); // Se llama automáticamente al método toString()

      
        Revista revista = new Revista("Java Magazine", "Editorial XYZ", "Informática", "Mensual", "1234-5678");
        System.out.println("\nInformación de la Revista:");
        System.out.println(revista); // Se llama automáticamente al método toString()

        
        Libro libro = new Libro("Introducción a Java", "John Doe", "978-0123456789", 300);
        System.out.println("\nInformación del Libro:");
        System.out.println(libro); // Se llama automáticamente al método toString()

      
        Periodico periodico = new Periodico("El País", "Grupo Prisa", "Actualidad", "01/05/2024");
        System.out.println("\nInformación del Periódico:");
        System.out.println(periodico); // Se llama automáticamente al método toString()
    }
}
