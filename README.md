

<!---
maregajr12/maregajr12 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
// pp_fp06.pizza_restaurant.enums.TamanhoPizza.java
package pp_fp06.pizza_restaurant.enums;

public enum TamanhoPizza {
    PEQUENA("Small size"),
    MEDIA("Medium size"),
    FAMILIAR("Big size");

    private final String description;

    TamanhoPizza(String description) {
        this.description = description;
    }

    public String getDescription() {
        return description;
    }

    // Método para converter o valor do enumerador em um formato legível
    public static String pizzaToString(TamanhoPizza tamanho) {
        switch (tamanho) {
            case PEQUENA:
                return "A pizza é pequena.";
            case FAMILIAR:
                return "A pizza é grande.";
            default:
                return "A pizza é média.";
        }
    }
}

// pp_fp06.pizza_restaurant.enums.OrigemIngrediente.java
package pp_fp06.pizza_restaurant.enums;

public enum OrigemIngrediente {
    ANIMAL("Animal"),
    VEGETAL("Vegetal"),
    MINERAL("Mineral");

    private final String description;

    OrigemIngrediente(String description) {
        this.description = description;
    }

    public String getDescription() {
        return description;
    }
}

// pp_fp06.pizza_restaurant.Ingrediente.java
package pp_fp06.pizza_restaurant;

import pp_fp06.pizza_restaurant.enums.OrigemIngrediente;

public class Ingrediente {
    private int codigo;
    private String nome;
    private OrigemIngrediente origem;
    private int numeroCalorias;

    // construtor, getters e setters

    // outros métodos se necessário
}

// pp_fp06.pizza_restaurant.Pizza.java
package pp_fp06.pizza_restaurant;

import pp_fp06.pizza_restaurant.enums.TamanhoPizza;

import java.util.ArrayList;

public class Pizza {
    private int codigo;
    private String nome;
    private String descricao;
    private double preco;
    private TamanhoPizza tamanho;
    private int numeroIngredientes;
    private ArrayList<Ingrediente> ingredientes;

    // construtor, getters e setters

    // outros métodos se necessário
}

// pp_fp06.pizza_restaurant.Ementa.java
package pp_fp06.pizza_restaurant;

import pp_fp06.pizza_restaurant.enums.TamanhoPizza;

import java.util.ArrayList;
import java.util.Date;

public class Ementa {
    private String designacao;
    private String descricao;
    private int codigoIdentificacao;
    private Date dataInicio;
    private Date dataFim;
    private int numeroPizzas;
    private ArrayList<Pizza> pizzas;

    // construtor, getters e setters

    // outros métodos se necessário
}

